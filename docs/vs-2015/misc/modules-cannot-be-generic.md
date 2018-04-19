---
title: "Modules cannot be generic | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "BC32073"
  - "vbc32073"
helpviewer_keywords: 
  - "BC32073"
ms.assetid: 47246e2b-51d4-4a10-a3ac-bc77b44fa2ca
caps.latest.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# Modules cannot be generic
A `Module` statement uses the `Of` keyword to introduce generic type parameters.  
  
 You can define and use generic classes, structures, interfaces, procedures, and delegates. You cannot define generic modules.  
  
 **Error ID:** BC32073  
  
### To correct this error  
  
1.  Remove the `Of` keyword from the `Module` statement.  
  
2.  If you want the functionality of a generic module, the closest approximation is a generic class. Use a [Class Statement](../Topic/Class%20Statement%20\(Visual%20Basic\).md) instead of a `Module` statement.  
  
## See Also  
 [Module Statement](../Topic/Module%20Statement.md)   
 [Of](../Topic/Of%20Clause%20\(Visual%20Basic\).md)   
 [Generic Types in Visual Basic](../Topic/Generic%20Types%20in%20Visual%20Basic%20\(Visual%20Basic\).md)   
 [How to: Define a Class That Can Provide Identical Functionality on Different Data Types](../Topic/How%20to:%20Define%20a%20Class%20That%20Can%20Provide%20Identical%20Functionality%20on%20Different%20Data%20Types%20\(Visual%20Basic\).md)