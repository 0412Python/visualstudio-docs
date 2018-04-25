---
title: "Statement cannot appear within an interface body | Microsoft Docs"
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
  - "vbc30603"
  - "BC30603"
helpviewer_keywords: 
  - "BC30603"
ms.assetid: 3aef29d6-eadf-4f1f-b214-dfeae5e51c4f
caps.latest.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# Statement cannot appear within an interface body
The declaration of an interface member includes a statement terminating the member, of the form `End`*membername*.  
  
 An interface defines only the signature of its members. Consequently, procedures and properties defined in an interface have only their initial line, specifying the name and signature. You do not include any code, internal declarations, or an `End Function`, `End Property`, or `End Sub` statement inside the interface.  
  
 **Error ID:** BC30603  
  
### To correct this error  
  
-   Remove the `End`*membername* statement from the interface definition.  
  
## See Also  
 [Interface Statement](http://msdn.microsoft.com/library/8997af73-bda3-4f79-bd41-ca396b610260)   
 [End \<keyword> Statement](http://msdn.microsoft.com/library/42d6e088-ab0f-4cda-88e8-fdce3e5fcf4f)