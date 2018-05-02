---
title: "-ResetAddin (devenv.exe) | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-general"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "disable addin"
  - "addin state"
  - "reset addin"
ms.assetid: 9e339c8d-d768-4d86-8f45-2f479fc8255b
caps.latest.revision: 9
author: "kempb"
ms.author: "kempb"
manager: "ghogen"
---
# /ResetAddin (devenv.exe)
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [-ResetAddin (devenv.exe)](https://docs.microsoft.com/visualstudio/ide/reference/resetaddin-devenv-exe).  
  
  
Removes commands and command UI associated with the specified Add-in.  
  
## Syntax  
  
```  
Devenv /ResetAddin AddIn  
```  
  
## Arguments  
 `AddIn`  
 Optional. The command name of the Add-in.  
  
## Remarks  
 By default, the command name of the add-in is equal to *\<AddInSolutionName>*.Connect*.\<AddInSolutionName>*, and appears in Connect.cs as the `commandName` parameter of the `Exec` method. You can also verify the command name by starting to type the name of the add-in into the Commands window in Visual Studio, and using Intellisense to fill in the rest.  
  
## Example  
 The following example starts Visual Studio and prevents the `MyAddin` add-in from running at startup.  
  
```  
Devenv.exe /ResetAddin MyAddin.Connect.MyAddin  
```  
  
## See Also  
 [Customizing Development Settings in Visual Studio](http://msdn.microsoft.com/en-us/22c4debb-4e31-47a8-8f19-16f328d7dcd3)   
 [Devenv Command Line Switches](../../ide/reference/devenv-command-line-switches.md)



