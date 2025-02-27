---
title: "Dictionary.Add(TKey, TValue) Method"
description: "Adds the specified key and value to the dictionary."
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
# Dictionary.Add(TKey, TValue) Method
> **Version**: _Available or changed with runtime version 1.0._

Adds the specified key and value to the dictionary.


## Syntax
```AL
[Ok := ]  Dictionary.Add(Key: TKey, Value: TValue)
```
## Parameters
*Dictionary*  
&emsp;Type: [Dictionary](dictionary-data-type.md)  
An instance of the [Dictionary](dictionary-data-type.md) data type.  

*Key*  
&emsp;Type: [TKey](dictionary-data-type.md)  
The key of the element to add.  

*Value*  
&emsp;Type: [TValue](dictionary-data-type.md)  
The value of the element to add.  


## Return Value
*[Optional] Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the operation was successful; otherwise **false**.   If you omit this optional return value and the operation does not execute successfully, a runtime error will occur.  


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[Dictionary Data Type](dictionary-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)