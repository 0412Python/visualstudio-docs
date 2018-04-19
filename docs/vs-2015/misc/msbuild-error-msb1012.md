---
title: "MSBuild Error MSB1012 | Microsoft Docs"
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
  - "MSBuild.MissingResponseFileError"
helpviewer_keywords: 
  - "MSB1012"
ms.assetid: 6e09e21d-9f64-4a8c-adec-f8efb28b7ac2
caps.latest.revision: 10
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# MSBuild Error MSB1012
**Specify a response file.**  
  
 A response file must be specified for the @ switch.  
  
### To correct this error  
  
-   Specify a response file. The syntax is @\<file name>, for example, `@BuildHW.txt`  
  
-   Do not include the @ switch on the command line.  
  
## See Also  
 [Command-Line Reference](../msbuild/msbuild-command-line-reference.md)