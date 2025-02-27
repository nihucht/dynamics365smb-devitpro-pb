---
title: "XmlDocument.ReadFrom(InStream, XmlReadOptions, var XmlDocument) Method"
description: "Reads and parses the XML document from the given data source."
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
# XmlDocument.ReadFrom(InStream, XmlReadOptions, var XmlDocument) Method
> **Version**: _Available or changed with runtime version 1.0._

Reads and parses the XML document from the given data source.


## Syntax
```AL
[Ok := ]  XmlDocument.ReadFrom(InStream: InStream, ReadOptions: XmlReadOptions, var Result: XmlDocument)
```
## Parameters
*InStream*  
&emsp;Type: [InStream](../instream/instream-data-type.md)  
A stream containing an XML document.  

*ReadOptions*  
&emsp;Type: [XmlReadOptions](../xmlreadoptions/xmlreadoptions-data-type.md)  
Specifies options for customizing how the document is parsed.  

*Result*  
&emsp;Type: [XmlDocument](xmldocument-data-type.md)  
The XmlDocument parsed from the given data source.  


## Return Value
*[Optional] Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the operation was successful; otherwise **false**.   If you omit this optional return value and the operation does not execute successfully, a runtime error will occur.  


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[XmlDocument Data Type](xmldocument-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)