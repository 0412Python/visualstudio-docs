---
title: "CLS Compliance Warning CLS09911 | Microsoft Docs"
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
  - "CLS09911"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "CLS09911"
ms.assetid: 8cc0b0c0-a823-4392-9bf9-4d12242ef451
caps.latest.revision: 8
author: "corob-msft"
ms.author: "corob"
manager: "douge"
---
# CLS Compliance Warning CLS09911
Generic types are not CLS-compliant  
  
 A CLS-compliant type cannot also be a generic type.  For more information about generics in Visual C++, see [Support for Generics in C++](http://msdn.microsoft.com/library/c7ccc316-a411-4c00-b2e2-f0c0eadc6cfd).  
  
 For more information Common Language Subset (CLS) compliance checking, see [CLS Compliant Assemblies](http://msdn.microsoft.com/en-us/3320b57e-ea55-4697-a17d-f509a36a3c93).  
  
 The following sample generates CLS09911:  
  
```  
// CLS09911.cpp  
// compile with: /clr /LD  
using namespace System;  
using namespace System::Reflection;  
[assembly:CLSCompliant (true)];  
[assembly:AssemblyKeyFile("clscompliance.snk")];  
  
generic <class T>  
public ref class Five {   // CLS09911  
};  
  
```