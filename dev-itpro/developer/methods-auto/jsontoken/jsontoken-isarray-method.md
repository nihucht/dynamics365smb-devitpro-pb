---
title: "JsonToken.IsArray() Method"
description: "Indicates whether a JsonToken represents a JSON array."
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
# JsonToken.IsArray() Method
> **Version**: _Available or changed with runtime version 1.0._

Indicates whether a JsonToken represents a JSON array.


## Syntax
```AL
Ok :=   JsonToken.IsArray()
```
> [!NOTE]
> This method can be invoked using property access syntax.
## Parameters
*JsonToken*  
&emsp;Type: [JsonToken](jsontoken-data-type.md)  
An instance of the [JsonToken](jsontoken-data-type.md) data type.  

## Return Value
*Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the JsonToken represents a JSON array; otherwise, **false**.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[JsonToken Data Type](jsontoken-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)