---
title: "The folder &#39;folder&#39; could not be added to the project. &lt;reason&gt; | Microsoft Docs"
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
  - "vs.tasklisterror.projfile_no_add_folder"
ms.assetid: 3f6a5aa7-17cc-4e78-93b7-96e0970e111e
caps.latest.revision: 7
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# The folder &#39;folder&#39; could not be added to the project. &lt;reason&gt;
A folder read from the .vbproj or .csproj file cannot be added to the project. Reasons include:  
  
-   Invalid name  
  
-   File within a path. For example, if you have a project-relative path of Folder1\Folder2\Folder3, but there is also a file with relative path Folder1\Folder2.  
  
-   Item already exists. This occurs when a folder is listed twice in the project file.  
  
 This error is most likely caused by editing the project file by hand.  
  
 **To correct this error**  
  
-   Remove the affected folder node from the project file.  
  
     Any folder, and any files below the folder, for which this diagnostic is displayed will not be added to the project.  
  
## See Also  
 [Project Files](http://msdn.microsoft.com/library/5261cf45-3136-40a6-899e-dc1339551401)   
 [NIB: Project Properties (Visual Studio)](http://msdn.microsoft.com/en-us/eb4c97ed-f667-4850-98d0-6e2a4d21bbca)