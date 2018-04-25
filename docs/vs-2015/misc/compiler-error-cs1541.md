---
title: "Compiler Error CS1541 | Microsoft Docs"
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
  - "CS1541"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS1541"
ms.assetid: db3350fe-6432-4617-8b4a-64bc6cdf83f8
caps.latest.revision: 9
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# Compiler Error CS1541
Invalid reference option: 'symbol' — cannot reference directories  
  
 The compiler detected an attempt to specify a directory rather than a specific file. For example, when you use the [/reference](http://msdn.microsoft.com/library/8d13e5b0-abf6-4c46-bf71-2daf2cd0a6c4) compiler option, you must specify a file; it is not possible to specify a directory.  
  
 For example, passing `/reference:c:\` to the compiler would generate CS1541.