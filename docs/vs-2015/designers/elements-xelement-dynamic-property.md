---
title: "Elements (XElement Dynamic Property) | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
api_name: 
  - "XElement.Elements"
api_type: 
  - "Assembly"
ms.assetid: 3d5737f2-d2ed-410a-821c-349dbb2b574f
caps.latest.revision: 4
author: "kempb"
ms.author: "kempb"
manager: "ghogen"
---
# Elements (XElement Dynamic Property)
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

The latest version of this topic can be found at [Elements (XElement Dynamic Property)](https://docs.microsoft.com/visualstudio/designers/elements-xelement-dynamic-property).  
  
Gets an indexer used to retrieve the child elements of the current element that match the specified expanded name.  
  
## Syntax  
  
```  
elem.Elements[{namespaceName}localName]   
```  
  
## Property Value/Return Value  
 An indexer of the type `IEnumerable<XElement> Item(String expandedName)`. This indexer takes the expanded name of the desired child elements and returns the matching child elements in an <xref:System.Collections.IEnumerable>`<`<xref:System.Xml.Linq.XElement>`>` collection.  
  
## Remarks  
 This property is equivalent to the <xref:System.Xml.Linq.XContainer.Elements%28System.Xml.Linq.XName%29?displayProperty=fullName> method of the <xref:System.Xml.Linq.XContainer> class.  
  
 The elements in the returned collection are in XML source document order.  
  
 This property uses deferred execution.  
  
## See Also  
 [XElement Class Dynamic Properties](../designers/xelement-class-dynamic-properties.md)   
 [Element](../designers/element-xelement-dynamic-property.md)   
 [Descendants](../designers/descendants-xelement-dynamic-property.md)



