---
title: "Compiler Warning (level 3) CS0067 | Microsoft Docs"
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
  - "CS0067"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0067"
ms.assetid: df75220b-0b93-45ec-8655-98d9333b0bb7
caps.latest.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# Compiler Warning (level 3) CS0067
The event 'event' is never used  
  
 An [event](http://msdn.microsoft.com/library/7858fd85-153b-4259-85d0-6aa13c35f174) was declared but never used in the class in which it was declared.  
  
 The following sample generates CS0067:  
  
```  
// CS0067.cs  
// compile with: /W:3  
using System;  
delegate void MyDelegate();  
  
class MyClass  
{  
   public event MyDelegate evt;   // CS0067  
   // uncomment TestMethod to resolve this CS0067  
/*  
   private void TestMethod()  
   {  
      if (evt != null)  
         evt();  
   }  
*/  
   public static void Main()  
   {  
   }  
}  
```