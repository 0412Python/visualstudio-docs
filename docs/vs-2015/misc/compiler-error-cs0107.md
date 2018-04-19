---
title: "Compiler Error CS0107 | Microsoft Docs"
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
  - "CS0107"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0107"
ms.assetid: 505763c5-6d68-4c57-a8bd-7b03682da4c5
caps.latest.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# Compiler Error CS0107
More than one protection modifier  
  
 Only one access modifier ([public](../Topic/public%20\(C%23%20Reference\).md), [private](../Topic/private%20\(C%23%20Reference\).md), [protected](../Topic/protected%20\(C%23%20Reference\).md), or [internal](../Topic/internal%20\(C%23%20Reference\).md)) is allowed on a class member, with the exception of except **internal protected**.  
  
 The following sample generates CS0107:  
  
```  
// CS0107.cs  
public class C  
{  
   private internal void f()   // CS0107, delete private or internal  
   {  
   }  
  
   public static int Main()  
   {  
      return 1;  
   }  
}  
```