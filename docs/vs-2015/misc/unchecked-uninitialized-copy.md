---
title: "unchecked_uninitialized_copy | Microsoft Docs"
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
  - "std.unchecked_uninitialized_copy"
  - "unchecked_uninitialized_copy"
  - "std::unchecked_uninitialized_copy"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "unchecked_uninitialized_copy function"
ms.assetid: 38568841-314e-446b-91d0-92cc231e3b3c
caps.latest.revision: 9
author: "ghogen"
ms.author: "ghogen"
manager: "douge"
---
# unchecked_uninitialized_copy
Same as [uninitialized_copy](http://msdn.microsoft.com/library/23a09cb8-4116-475e-b0bb-5d3e7daca5aa) but allows the use of an unchecked iterator as output iterator when _SECURE_SCL=1 is defined. This function is defined in the [stdext Namespace](http://msdn.microsoft.com/library/3e94fc89-0584-424f-bc09-081b73379545) namespace.  
  
> [!NOTE]
>  This algorithm is a Microsoft extension to the Standard C++ Library. Code implemented using this algorithm will not be portable.  
  
## Syntax  
  
```  
template<class InputIterator, class ForwardIterator>  
   ForwardIterator unchecked_uninitialized_copy(  
      InputIterator _First,  
      InputIterator _Last,  
      ForwardIterator _Dest  
   );  
  
template<class InputIterator, class ForwardIterator, class Allocator>  
   ForwardIterator unchecked_uninitialized_copy(  
      InputIterator _First,  
      InputIterator _Last,  
      ForwardIterator _Dest,  
      Allocator& _Al  
   );  
```  
  
#### Parameters  
 `_First`  
 An input iterator addressing the first element in the source range to be copied.  
  
 `_Last`  
 An input iterator addressing the last element in the source range to be copied.  
  
 `_Dest`  
 A forward iterator addressing the first element in the destination range to be copied.  
  
 `_Al`  
 The allocator class to use with this object. [vector::get_allocator](http://msdn.microsoft.com/library/1570bc99-914a-486b-8846-fb0a6ed289a4) returns the allocator class for the object.  
  
## Return Value  
 A forward iterator addressing the position one past the final element in the destination range that is receiving the copy.  
  
## Remarks  
 See [uninitialized_copy](http://msdn.microsoft.com/library/23a09cb8-4116-475e-b0bb-5d3e7daca5aa) for a code sample.  
  
 For more information on checked iterators, see [Checked Iterators](http://msdn.microsoft.com/library/cfc87df8-e3d9-403b-ab78-e9483247d940).  
  
## Requirements  
 **Header:** \<memory>  
  
 **Namespace:** stdext