---
title: "Compiler Error CS0254 | Microsoft Docs"
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
  - "CS0254"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0254"
ms.assetid: 85b2ab1e-0011-4f1d-9181-76b9c9f3d914
caps.latest.revision: 8
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# Compiler Error CS0254
The right hand side of a fixed statement assignment may not be a cast expression  
  
 The right side of a [fixed](http://msdn.microsoft.com/library/7ea6db08-ad49-4a7a-b934-d8c4acad1c3a) expression may not use a cast. For more information, see [Unsafe Code and Pointers](http://msdn.microsoft.com/library/b0fcca10-a92d-4f2a-835b-b0ccae6739ee).  
  
 The following sample generates CS0254:  
  
```  
// CS0254.cs  
// compile with: /unsafe  
class Point  
{  
   public uint x, y;  
}  
  
class FixedTest  
{  
   unsafe static void SquarePtrParam (int* p)  
   {  
      *p *= *p;  
   }  
  
   unsafe public static void Main()  
   {  
      Point pt = new Point();  
      pt.x = 5;  
      pt.y = 6;  
  
      fixed (int* p = (int*)&pt.x)   // CS0254  
      // try the following line instead  
      // fixed (uint* p = &pt.x)  
      {  
         SquarePtrParam ((int*)p);  
      }  
   }  
}  
```