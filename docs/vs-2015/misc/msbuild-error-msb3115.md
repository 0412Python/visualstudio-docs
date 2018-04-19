---
title: "MSBuild Error MSB3115 | Microsoft Docs"
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
  - "MSBuild.GenerateManifest.InvalidEntryPoint"
helpviewer_keywords: 
  - "MSB3115"
ms.assetid: 7d9d4156-fd6a-455a-8a3d-b191485f1294
caps.latest.revision: 5
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# MSBuild Error MSB3115
**MSB3115: File '\<file>' is not a valid entry point.**  
  
 This error is generated when a manifest specifies an entry point that is not valid.  
  
### To correct this error  
  
-   Be sure that you specify valid entry points in your manifests. For an application manifest, a valid entry point is an .exe file. For a deployment manifest, a valid entry point is an application manifest.