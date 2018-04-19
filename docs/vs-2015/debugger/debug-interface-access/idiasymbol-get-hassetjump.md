---
title: "IDiaSymbol::get_hasSetJump | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "IDiaSymbol::get_hasSetJump method"
ms.assetid: 22656206-dccf-40ed-b179-fc016d1b262a
caps.latest.revision: 10
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaSymbol::get_hasSetJump
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDiaSymbol::get_hasSetJump](https://docs.microsoft.com/visualstudio/debugger/debug-interface-access/idiasymbol-get-hassetjump).  
  
Retrieves a flag that specifies whether the function contains a use of the [setjmp](../Topic/setjmp.md) command (paired with the [longjmp](../Topic/longjmp.md) command, these form the C-style method of exception handling).  
  
## Syntax  
  
```cpp  
HRESULT get_hasSetJump(  
   BOOL *pFlag  
);  
```  
  
#### Parameters  
 `pFlag`  
 [out] Returns `TRUE` if the function contains a `setjmp` command; otherwise, returns `FALSE`.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or error code.  
  
> [!NOTE]
>  A return value of `S_FALSE` means the property is not available for the symbol.  
  
## Requirements  
  
|Requirement|Description|  
|-----------------|-----------------|  
|Header:|dia2.h|  
|Version:|DIA SDK v8.0|  
  
## See Also  
 [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)   
 [IDiaSymbol::get_hasLongJump](../../debugger/debug-interface-access/idiasymbol-get-haslongjump.md)   
 [longjmp](../Topic/longjmp.md)   
 [setjmp](../Topic/setjmp.md)



