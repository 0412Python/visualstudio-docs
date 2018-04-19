---
title: "Member &#39;&lt;membername&gt;&#39; cannot be initialized in an object initializer expression because it is shared | Microsoft Docs"
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
  - "bc30991"
  - "vbc30991"
helpviewer_keywords: 
  - "BC30991"
ms.assetid: 47e832b4-47e3-426e-b88c-5d5568102fde
caps.latest.revision: 12
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# Member &#39;&lt;membername&gt;&#39; cannot be initialized in an object initializer expression because it is shared
Object initializers cannot be used to initialize any member of a class that is declared as shared. For more information, see [Shared](http://msdn.microsoft.com/library/2bf7cf2c-b0dd-485e-8749-b5d674dab4cd).  
  
 **Error ID:** BC30991  
  
### To correct this error  
  
1.  Examine the class definition to determine which member is shared.  
  
2.  Eliminate the initialization for that member from the object initializer list.  
  
## Example  
 In the following example, `totalCustomers` is a shared member.  
  
```  
Public Class Customer  
    Public Shared totalCustomers As Integer  
    ' Other declarations and method definitions.  
End Class  
```  
  
 Because `totalCustomers` is shared, trying to set its initial value in an object initializer list causes this error.  
  
```  
' This declaration is not valid.  
' Dim cust As New Customer With { .Name = "Coho Winery", _  
'                                 .totalCustomers = 21 }  
```  
  
## See Also  
 [Object Initializers: Named and Anonymous Types](http://msdn.microsoft.com/library/e2df3807-a70f-49dd-ac94-f1e07f472b1b)   
 [Shared](http://msdn.microsoft.com/library/2bf7cf2c-b0dd-485e-8749-b5d674dab4cd)   
 [NOT IN BUILD: Shared Members in Visual Basic](http://msdn.microsoft.com/en-us/dbc3783f-83a2-4225-995d-c2d6d025663d)