---
title: "&#39;WriteOnly&#39; property must provide a &#39;Set&#39; | Microsoft Docs"
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
  - "bc30125"
  - "vbc30125"
helpviewer_keywords: 
  - "BC30125"
ms.assetid: c2b18086-9cd9-4094-b9a9-491c8d617096
caps.latest.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# &#39;WriteOnly&#39; property must provide a &#39;Set&#39;
If a property is declared as `WriteOnly`, it must supply a procedure for writing its value.  
  
 **Error ID:** BC30125  
  
### To correct this error  
  
1.  Make sure you include a `Set` procedure between the `Property` statement and the `End Property` statement.  
  
2.  Verify that other procedures within the `Property` declaration are correctly terminated.  
  
## See Also  
 [Property Statement](../Topic/Property%20Statement.md)   
 [Set Statement](../Topic/Set%20Statement%20\(Visual%20Basic\).md)