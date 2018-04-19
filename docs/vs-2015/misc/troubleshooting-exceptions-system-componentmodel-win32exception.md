---
title: "Troubleshooting Exceptions: System.ComponentModel.Win32Exception | Microsoft Docs"
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
  - "Win32Exception exception"
  - "System.ComponentModel.Win32Exception exception"
ms.assetid: 6d5facbd-34f0-4f04-a7df-2bf62d676529
caps.latest.revision: 4
author: "mikeblome"
ms.author: "mblome"
manager: "douge"
---
# Troubleshooting Exceptions: System.ComponentModel.Win32Exception
The exception that is thrown for a Win32 error code.  
  
## Remarks  
 Win32 error codes are translated from their numeric representations into a system message when they are displayed. Use the <xref:System.ComponentModel.Win32Exception.NativeErrorCode%2A> property to access the numeric representation of the error code.  
  
## See Also  
 <xref:System.ComponentModel.Win32Exception>   
 [Use the Exception Assistant](http://msdn.microsoft.com/library/e0a78c50-7318-4d54-af51-40c00aea8711)   
 [Where Can I Look Up Win32 Error Codes?](../debugger/where-can-i-look-up-win32-error-codes-q.md)