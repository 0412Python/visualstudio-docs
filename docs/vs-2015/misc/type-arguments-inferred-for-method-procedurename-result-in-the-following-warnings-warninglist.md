---
title: "Type arguments inferred for method &#39;&lt;procedurename&gt;&#39; result in the following warnings :&lt;warninglist&gt; | Microsoft Docs"
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
  - "bc41006"
  - "vbc41006"
helpviewer_keywords: 
  - "BC41006"
ms.assetid: c789ffa9-0273-47f6-8915-78fc6a7d3d6d
caps.latest.revision: 6
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# Type arguments inferred for method &#39;&lt;procedurename&gt;&#39; result in the following warnings :&lt;warninglist&gt;
A generic procedure is called without supplying any type arguments, and the inferred type arguments result in one or more warnings.  
  
 Normally, when you invoke a generic type, you supply a type argument for each type parameter that the generic type defines. If you do not supply any type arguments, the compiler attempts to infer the types to be passed to the type parameters. If the inferred types cause ambiguity, or if they create a situation that could lead to unexpected results, then the compiler generates this warning.  
  
 A *constraint* on a type parameter limits what type arguments can be passed to it. For example, a type parameter might be constrained to be a class that implements the <xref:System.IComparable%601> interface. For more information, see "Constraints" in [Generic Procedures in Visual Basic](http://msdn.microsoft.com/library/95577b28-137f-4d5c-a149-919c828600e5).  
  
 By default, this message is a warning. For information on hiding warnings or treating warnings as errors, see [Configuring Warnings in Visual Basic](../ide/configuring-warnings-in-visual-basic.md).  
  
 **Error ID:** BC41006  
  
### To correct this error  
  
-   Supply type arguments to the generic procedure so that the compiler does not have to infer them.  
  
## See Also  
 [Generic Types in Visual Basic](http://msdn.microsoft.com/library/89f771d9-ecbb-4737-88b8-116b63c6cf4d)   
 [Generic Procedures in Visual Basic](http://msdn.microsoft.com/library/95577b28-137f-4d5c-a149-919c828600e5)   
 [Type List](http://msdn.microsoft.com/library/56db947a-2ae8-40f2-a70a-960764e9d0db)