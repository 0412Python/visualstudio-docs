---
title: "One or more selected items contain a data type that is not supported by the designer | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 71dcd4f9-2946-42c5-9ce4-99c819ea2785
caps.latest.revision: 8
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
---
# One or more selected items contain a data type that is not supported by the designer
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [One or more selected items contain a data type that is not supported by the designer](https://docs.microsoft.com/visualstudio/data-tools/one-or-more-selected-items-contain-a-data-type-that-is-not-supported-by-the-designer).  
  
  
One or more of the items dragged from **Server Explorer**/**Database Explorer** onto the [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)] contains a data type that is not supported by the [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)] (for example, [CLR User-Defined Types](../Topic/CLR%20User-Defined%20Types.md)).  
  
### To correct this error  
  
1.  Create a view that is based on the desired table and that does not include the unsupported data type.  
  
2.  Drag the view from **Server Explorer**/**Database Explorer** onto the designer.  
  
## See Also  
 [LINQ to SQL Tools in Visual Studio](../data-tools/linq-to-sql-tools-in-visual-studio2.md)   
 [Walkthrough: Creating LINQ to SQL Classes (O-R Designer)](../Topic/Walkthrough:%20Creating%20LINQ%20to%20SQL%20Classes%20\(O-R%20Designer\).md)   
 [LINQ to SQL](../Topic/LINQ%20to%20SQL.md)

