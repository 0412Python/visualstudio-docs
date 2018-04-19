---
title: "Error: Firewall on Local Machine | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vs.debug.error.firewall.localmachine"
dev_langs: 
  - "FSharp"
  - "VB"
  - "CSharp"
  - "C++"
ms.assetid: ab60dda9-7934-4891-aa2f-001380d2ed83
caps.latest.revision: 10
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# Error: Firewall on Local Machine
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [Error: Firewall on Local Machine](https://docs.microsoft.com/visualstudio/debugger/error-firewall-on-local-machine).  
  
The Internet Connection Firewall on the local machine, the machine you are running Visual Studio from, is not set up to allow remote debugging. For managed or native remote debugging with the default transport, the TCP 135 port must be opened for DCOM traffic. File and printer sharing must be opened, and devenv.exe must be added to the exceptions list. Opening some IPSEC ports may be necessary as well.  
  
 For more information, see [Set Up the Remote Tools on the Device](../Topic/Set%20Up%20the%20Remote%20Tools%20on%20the%20Device.md).



