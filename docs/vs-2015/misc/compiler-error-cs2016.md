---
title: "Compiler Error CS2016 | Microsoft Docs"
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
  - "CS2016"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS2016"
ms.assetid: 69f77502-f726-4856-ac87-e556eeb67349
caps.latest.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# Compiler Error CS2016
Code page 'codepage' is invalid or not installed  
  
 The [/codepage](http://msdn.microsoft.com/library/75942989-b69a-4308-90a0-840c73d2c478) compiler option was passed an invalid value.  
  
 The following sample generates CS2016:  
  
```  
// CS2016.cs  
// compile with: /codepage:x  
// CS2016 expected  
class MyClass  
{  
   public static void Main()  
   {  
   }  
}  
```