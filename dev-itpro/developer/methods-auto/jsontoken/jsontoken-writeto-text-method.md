---
title: "JsonToken.WriteTo(var Text) Method"
description: "Serializes and writes the JSON data of the JsonToken to a given Text object."
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
# JsonToken.WriteTo(var Text) Method
> **Version**: _Available or changed with runtime version 1.0._

Serializes and writes the JSON data of the JsonToken to a given Text object.


## Syntax
```AL
[Ok := ]  JsonToken.WriteTo(var String: Text)
```
## Parameters
*JsonToken*  
&emsp;Type: [JsonToken](jsontoken-data-type.md)  
An instance of the [JsonToken](jsontoken-data-type.md) data type.  

*String*  
&emsp;Type: [Text](../text/text-data-type.md)  
The Text object to which the JSON data will be read.  


## Return Value
*[Optional] Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the read was successful; otherwise, **false**. If you omit this optional return value and the operation does not execute successfully, a runtime error will occur.  


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[JsonToken Data Type](jsontoken-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)