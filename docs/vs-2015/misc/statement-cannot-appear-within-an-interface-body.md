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
 [Interface Statement](../Topic/Interface%20Statement%20\(Visual%20Basic\).md)   
 [End \<keyword> Statement](../Topic/End%20%3Ckeyword%3E%20Statement%20\(Visual%20Basic\).md)