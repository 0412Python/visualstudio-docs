---
title: "CA2137: Transparent methods must contain only verifiable IL | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-devops-test"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "CA2137"
ms.assetid: cbaeb0e1-56b6-43b4-812a-596b2859c329
caps.latest.revision: 15
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# CA2137: Transparent methods must contain only verifiable IL
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [CA2137: Transparent methods must contain only verifiable IL](https://docs.microsoft.com/visualstudio/code-quality/ca2137-transparent-methods-must-contain-only-verifiable-il).  
  
TypeName|TransparentMethodsMustBeVerifiable|  
|CheckId|CA2137|  
|Category|Microsoft.Security|  
|Breaking Change|Breaking|  
  
## Cause  
 A method contains unverifiable code or returns a type by reference.  
  
## Rule Description  
 This rule fires on attempts by security transparent code to execute unverifiable MSIL (Microsoft Intermediate Language). However, the rule does not contain a full IL verifier, and instead uses heuristics to catch most violations of MSIL verification.  
  
 To be certain that your code contains only verifiable MSIL, run [Peverify.exe (PEVerify Tool)](../Topic/Peverify.exe%20\(PEVerify%20Tool\).md) on your assembly. Run PEVerify with the **/transparent** option which limits the output to only unverifiable transparent methods which would cause an error. If the /transparent option is not used, PEVerify also verifies critical methods that are allowed to contain unverifiable code.  
  
## How to Fix Violations  
 To fix a violation of this rule, mark the method with the <xref:System.Security.SecurityCriticalAttribute> or <xref:System.Security.SecuritySafeCriticalAttribute> attribute, or remove the unverifiable code.  
  
## When to Suppress Warnings  
 Do not suppress a warning from this rule.  
  
## Example  
 The method in this example uses unverifiable code and should be marked with the <xref:System.Security.SecurityCriticalAttribute> or <xref:System.Security.SecuritySafeCriticalAttribute> attribute.  
  
 [!code-csharp[FxCop.Security.CA2137.TransparentMethodsMustBeVerifiable#1](../snippets/csharp/VS_Snippets_CodeAnalysis/fxcop.security.ca2137.transparentmethodsmustbeverifiable/cs/ca2137 - transparentmethodsmustbeverifiable.cs#1)]



