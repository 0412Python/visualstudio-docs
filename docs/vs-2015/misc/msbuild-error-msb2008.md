---
title: "MSBuild Error MSB2008 | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "MSBuild.UnrecognizedChildElement"
helpviewer_keywords: 
  - "MSB2008"
ms.assetid: 3c2afda0-a116-4b2f-af0c-c0f0d1541325
caps.latest.revision: 13
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# MSBuild Error MSB2008
**The Visual Studio project system cannot convert "{0}" projects. It can only be used to convert C# and VB client projects.**  
  
 Only valid [!INCLUDE[vbprvb](../includes/vbprvb-md.md)] and [!INCLUDE[csprcs](../includes/csprcs-md.md)] projects can be converted using [!INCLUDE[vstecmsbuild](../includes/vstecmsbuild-md.md)].  
  
### To correct this error  
  
-   If the project is a [!INCLUDE[vbprvb](../includes/vbprvb-md.md)] or [!INCLUDE[csprcs](../includes/csprcs-md.md)] project, check whether the project file has been modified or corrupted. If it has been modified or corrupted, open the project in the version of [!INCLUDE[vsprvs](../includes/vsprvs-md.md)] in which it was created, save it, and then attempt to convert it again.  
  
-   If the project is not a [!INCLUDE[vbprvb](../includes/vbprvb-md.md)] or [!INCLUDE[csprcs](../includes/csprcs-md.md)] project, use the appropriate tool to convert it.  
  
## See Also  
 [Additional Resources](../msbuild/additional-msbuild-resources.md)