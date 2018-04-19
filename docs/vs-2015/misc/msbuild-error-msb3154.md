---
title: "MSBuild Error MSB3154 | Microsoft Docs"
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
  - "MSBuild.GenerateBootstrapper.ProductCultureNotFound"
helpviewer_keywords: 
  - "MSB3154"
ms.assetid: 513b70fa-15f5-4137-bdbc-5974607fb75a
caps.latest.revision: 6
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# MSBuild Error MSB3154
**MSB3154: Could not find string resources for item '\<package>'.**  
  
 This error is generated when the specified package does not contain any culture-specific information. Either a package.xml file does not exist, or it does not contain a `Culture` attribute.  
  
### To correct this error  
  
-   Provide a valid package.xml that contains a correct `Culture` tag.