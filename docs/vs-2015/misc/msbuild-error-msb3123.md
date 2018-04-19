---
title: "MSBuild Error MSB3123 | Microsoft Docs"
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
  - "GenerateManifest.FileAssociationsCountExceedsMaximum"
helpviewer_keywords: 
  - "MSB3123"
ms.assetid: 343aa8a8-9ab9-4dd5-be59-8eccf1f3c012
caps.latest.revision: 7
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# MSBuild Error MSB3123
**MSB3123: The number of file associations exceeds the limit of \<limit>.**  
  
 Each file is allowed only a fixed number of associated file name extensions. This error occurs when you try to associate more file name extensions than the number allowed for the target operating system.  
  
### To correct this error  
  
-   Limit the number of file associations to the specified number.  
  
## See Also  
 [Publish Page, Project Designer](../ide/reference/publish-page-project-designer.md)   
 [ClickOnce Application Manifest](../deployment/clickonce-application-manifest.md)