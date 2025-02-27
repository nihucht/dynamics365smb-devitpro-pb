---
title: "RecordRef.SystemCreatedAtNo() Method"
description: "Gets the field number that is used by the SystemCreatedAt field."
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
# RecordRef.SystemCreatedAtNo() Method
> **Version**: _Available or changed with runtime version 6.0._

Gets the field number that is used by the SystemCreatedAt field. The SystemCreatedAt field is a system field that the platform adds to all table objects.


## Syntax
```AL
SystemCreatedAtFieldNo :=   RecordRef.SystemCreatedAtNo()
```
> [!NOTE]
> This method can be invoked using property access syntax.
## Parameters
*RecordRef*  
&emsp;Type: [RecordRef](recordref-data-type.md)  
An instance of the [RecordRef](recordref-data-type.md) data type.  

## Return Value
*SystemCreatedAtFieldNo*  
&emsp;Type: [Integer](../integer/integer-data-type.md)  
The field number of the SystemCreatedAt field.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[RecordRef Data Type](recordref-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)