---
title: "HttpHeaders.GetValues(Text, Array of [Text]) Method"
description: "Gets the values for the specified key."
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
# HttpHeaders.GetValues(Text, Array of [Text]) Method
> **Version**: _Available or changed with runtime version 1.0._

Gets the values for the specified key.


## Syntax
```AL
[Ok := ]  HttpHeaders.GetValues(Key: Text, Values: Array of [Text])
```
## Parameters
*HttpHeaders*  
&emsp;Type: [HttpHeaders](httpheaders-data-type.md)  
An instance of the [HttpHeaders](httpheaders-data-type.md) data type.  

*Key*  
&emsp;Type: [Text](../text/text-data-type.md)  
The specified header.  

*Values*  
&emsp;Type: [Text](../text/text-data-type.md)  
The specified header values.  


## Return Value
*[Optional] Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the specified header name and values are stored in the collection; otherwise **false**. If you omit this optional return value and the operation does not execute successfully, a runtime error will occur.  


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[HttpHeaders Data Type](httpheaders-data-type.md)
[Get Started with AL](../../devenv-get-started.md)
[Developing Extensions](../../devenv-dev-overview.md)