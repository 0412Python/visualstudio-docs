---
title: "MSBuild Error MSB3113 | Microsoft Docs"
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
  - "MSBuild.GenerateManifest.ResolveFailedInReadWriteMode"
helpviewer_keywords: 
  - "MSB3113"
ms.assetid: 81e73738-e6ee-4651-9f48-acb1feef3ff5
caps.latest.revision: 6
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# MSBuild Error MSB3113
**MSB3113: Could not find file '\<file>'.**  
  
 This error is generated when an irresolvable reference is encountered when creating a new manifest. It might have originated from the project file or as a task parameter.  
  
### To correct this error  
  
-   Check your project file (and build parameters, if you are custom building) for conflicts in file references.  
  
## See Also  
 [\<PackageFiles> Element](../deployment/packagefiles-element-bootstrapper.md)