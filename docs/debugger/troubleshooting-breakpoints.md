---
title: "Troubleshoot Breakpoints in the Visual Studio Debugger | Microsoft Docs"
ms.custom: ""
ms.date: "01/23/2018"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "breakpoints, fixing breakpoints, breakpoint warnings"
ms.assetid: 6b4fa32a-7a97-41ef-b82d-61feaf9982b1
caps.latest.revision: 0
author: "carpediemma"
ms.author: "emrou"
manager: emrou
ms.workload: 
  - "multiple"
---
# Troubleshoot Breakpoints in the Visual Studio Debugger

## Breakpoint Warnings

When debugging, a breakpoint has two possible visual states: a solid red circle and a hollow (white filled) circle. If the debugger was able to successfully set a breakpoint in the target process, it will stay a solid red circle. If the breakpoint is a hollow circle, either the breakpoint is disabled or there was a warning when trying to set the breakpoint. To determine the difference, hover over the breakpoint and see if there is a warning.

The following two sections describe prominent warnings and how to fix them. 

### "No Symbols have been loaded for this document" 

Go to the **Modules** window (**Debug** > **Windows** > **Modules**) and check whether your module is loaded.  
* If your module is loaded, check the **Symbol Status** column to see whether symbols have been loaded. 
  * If symbols are not loaded, check the symbol status to diagnose the issue. From the context menu on a module in the **Modules** window, click on the **Symbol Load Information...** item to see where the debugger looked to try and load symbols. For more information about loading symbols, see [Specify Symbol (.pdb) and Source Files](../debugger/specify-symbol-dot-pdb-and-source-files-in-the-visual-studio-debugger.md).  
  * If symbols are loaded, this means that the PDB didn't contain information about your source files. These are a few possible causes: 
    * If your source files were recently added, confirm that an up-to-date version of the module is being loaded.  
    * It is possible to create stripped PDBs using the **/PDBSTRIPPED** linker option. Stripped PDBs do not contain source file information. Confirm you are working with a full PDB and not a stripped PDB.  
    * The PDB file is partially corrupted. Try deleting the file and doing a clean build of the module to see if this resolves the issue. 

* If your module is not loaded, check the following to find the cause: 
  * Confirm that you are debugging the right process. 
  * Check to see that you are debugging the right kind of code. You can find out what type of code the debugger is configured to debug in the **Processes** window (**Debug** > **Windows** > **Processes**). For example, if you are trying to debug C# code, confirm that your debugger is configured for the appropriate type of .NET Framework (e.g. Managed (v4\*) versus Managed (v2\*/v3\*) versus Managed (CoreCLR)). 

### "… the current source code is different from the version built into..." 

If a source file has changed and the source no longer matches the code you are debugging, the debugger will not set breakpoints in the code by default. Normally, this problem happens when a source file is changed, but the source code wasn’t rebuilt. To fix this issue, rebuild the project. If the build system thinks the project is already up to date even though it isn’t, you can force the project system to rebuild either by saving the source file again or by cleaning the project’s build output before building. 

In rare scenarios, you may want to debug without having matching source code. This can lead to a very confusing debugging experience, so ensure that this is how you want to proceed.  

To disable these safety checks, do one of the following: 
* To modify a single breakpoint, hover over the breakpoint icon in the editor and click the settings (gear) icon. A peak window will be added to the editor. At the top of the peak window there is a hyperlink that indicates the location of the breakpoint. Click the hyperlink to allow modification of the breakpoint location and check **Allow the source code to be different from the original**.
* To modify this setting for all breakpoints, go to **Debug** > **Options and Settings**. On the **Debugging/General** page, clear the **Require source files that exactly match the original version** option. Make sure to reenable this option once you are done debugging. 

## The breakpoint was successfully set (no warning), but didn’t hit 

This section provides information to troubleshoot issues when the debugger isn’t displaying any warnings – the breakpoint is a solid red circle while actively debugging, yet the breakpoint isn’t being hit. 

Here are a few things to check: 
1. If your code runs in more than one process or more than one computer, ensure that you are debugging the right process or computer.  
2. Confirm that your code is running. One easy way to test this is to add a call to `System.Diagnostics.Debugger.Break` (C#/VB) or `__debugbreak` (C++) to the line of code where you are trying to set the breakpoint and rebuild your project. 
3. If you are debugging optimized code, make sure the function where your breakpoint is set isn’t being inlined into another function. The `Debugger.Break` test mentioned in the previous check can work to test this as well. 

## I deleted a breakpoint, but I continue to hit it when I start debugging again 

If you deleted a breakpoint while debugging, you may hit the breakpoint again the next time you start debugging. To stop hitting this breakpoint, make sure all the instances of the breakpoint are removed from the **Breakpoints** window.  