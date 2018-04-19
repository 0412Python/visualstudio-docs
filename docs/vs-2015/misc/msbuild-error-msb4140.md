---
title: "MSBuild Error MSB4140 | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "MSB4140"
ms.assetid: 13546558-4ed4-44c2-89a6-f69a2b43ed07
caps.latest.revision: 8
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# MSBuild Error MSB4140
**MSB4140: Default ToolsVersion is specified in neither the registry nor configuration file.**  
  
 The project does not specify a default `ToolsVersion` value. Therefore, [!INCLUDE[vstecmsbuild](../includes/vstecmsbuild-md.md)] does not know which value to use.  
  
### To correct this error  
  
-   Make sure that a `DefaultToolsVersion` value is specified either in the registry where Toolsets are defined, or in a configuration file (such as msbuild.exe.config).  
  
## See Also  
 [Standard and Custom Toolset Configurations](../msbuild/standard-and-custom-toolset-configurations.md)   
 [Project Element (MSBuild)](../msbuild/project-element-msbuild.md)   
 [Additional Resources](../msbuild/additional-msbuild-resources.md)