---
title: "XML descendant elements cannot be selected from type &#39;type&#39; | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vbc36809"
  - "bc36809"
helpviewer_keywords: 
  - "BC36809"
ms.assetid: 560a3370-f24d-4ca3-93b1-39aabe13c238
caps.latest.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# XML descendant elements cannot be selected from type &#39;type&#39;
An XML descendant has been referenced for an object that is not of type <xref:System.Xml.Linq.XElement>, <xref:System.Xml.Linq.XDocument>, or `IEnumerable(Of XElement)`. For more information, see [XML Descendant Axis Property](../Topic/XML%20Descendant%20Axis%20Property%20\(Visual%20Basic\).md).  
  
```vb  
' Generates an error.  
Dim var = "sample text"...<childElement>  
```  
  
 **Error ID:** BC36809  
  
### To correct this error  
  
-   Ensure that the object of which you are referencing a descendant element is strongly typed as <xref:System.Xml.Linq.XElement>, <xref:System.Xml.Linq.XDocument>, or `IEnumerable(Of XElement)`. Following is an example:  
  
    ```vb  
    Dim elem As XElement = <root>  
                            <child />  
                           </root>  
    Dim var = elem...<child>  
    ```  
  
## See Also  
 [XML Descendant Axis Property](../Topic/XML%20Descendant%20Axis%20Property%20\(Visual%20Basic\).md)   
 [XML Axis Properties](../Topic/XML%20Axis%20Properties%20\(Visual%20Basic\).md)   
 [XML](../Topic/XML%20in%20Visual%20Basic.md)