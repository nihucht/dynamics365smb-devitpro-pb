---
title: "XmlDocument.GetDescendantElements(Text) Method"
description: "Gets a list containing the descendant elements for this document, in document order."
ms.author: solsen
ms.custom: na
ms.date: 02/26/2024
ms.tgt_pltfrm: na
ms.topic: reference
author: SusanneWindfeldPedersen
---
[//]: # (START>DO_NOT_EDIT)
[//]: # (IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT.)
[//]: # (Any modifications should be made in the .xml files in the ModernDev repo.)
# XmlDocument.GetDescendantElements(Text) Method
> **Version**: _Available or changed with runtime version 1.0._

Gets a list containing the descendant elements for this document, in document order.


## Syntax
```AL
DescendantElements :=   XmlDocument.GetDescendantElements(Name: Text)
```
## Parameters
*XmlDocument*  
&emsp;Type: [XmlDocument](xmldocument-data-type.md)  
An instance of the [XmlDocument](xmldocument-data-type.md) data type.  

*Name*  
&emsp;Type: [Text](../text/text-data-type.md)  
The fully qualified name of the elements to retrieve.  


## Return Value
*DescendantElements*  
&emsp;Type: [XmlNodeList](../xmlnodelist/xmlnodelist-data-type.md)  
A list containing the descendant elements for this document, in document order.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[XmlDocument Data Type](xmldocument-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)