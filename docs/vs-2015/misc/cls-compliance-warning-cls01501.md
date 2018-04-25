---
title: "CLS Compliance Warning CLS01501 | Microsoft Docs"
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
  - "CLS01501"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "CLS01501"
ms.assetid: 74361331-3773-48d5-8508-0113f5464a75
caps.latest.revision: 6
author: "corob-msft"
ms.author: "corob"
manager: "douge"
---
# CLS Compliance Warning CLS01501
**The varargs constraint is not part of the CLS**  
  
 The varargs constraint is not part of the Common Language Subset (CLS).  The only calling convention supported by the CLS is the standard managed calling convention.  
  
 For more information CLS compliance checking, see [CLS Compliant Assemblies](http://msdn.microsoft.com/en-us/3320b57e-ea55-4697-a17d-f509a36a3c93).  
  
 The following function declaration (using MSIL assembly language) shows what could cause CLS01501:  
  
```  
.method public specialname rtspecialname   
        instance vararg void  .ctor() cil managed  
```  
  
 You can resolve CLS01501 by using a parameter array.  See [Variable Argument Lists (...) (C++/CLI)](http://msdn.microsoft.com/library/db1a27f4-02a8-4318-8690-1f2893f52b38) for more information.