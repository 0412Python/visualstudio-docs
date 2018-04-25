---
title: "Using Memory Efficiently When You Build Large Projects | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "memory use (MSBuild)"
  - "msbuild, efficient memory use building large trees"
  - "caching (MSBuild)"
ms.assetid: 853a21ed-69f7-4817-af00-57f73e2c74b5
caps.latest.revision: 15
author: "kempb"
ms.author: "kempb"
manager: "ghogen"
---
# Using Memory Efficiently When You Build Large Projects
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [Using Memory Efficiently When You Build Large Projects](https://docs.microsoft.com/visualstudio/msbuild/using-memory-efficiently-when-you-build-large-projects).  
  
  
Large projects often contain many sub-projects and other dependencies, and these may consume lots of system memory at build time. When available system memory is decreased, system performance may also be decreased. Older versions of [!INCLUDE[vstecmsbuild](../includes/vstecmsbuild-md.md)] projects remained in memory or, in version 3.5 the projects were removed, but it retained build results in a cache for later retrieval.  
  
 Version 4.0 handles this memory management automatically, saving projects from having to use properties such as  `UnloadProjectsOnCompletion` and `UseResultsCache`.  
  
## See Also  
 [Building Multiple Projects in Parallel](../msbuild/building-multiple-projects-in-parallel-with-msbuild.md)



