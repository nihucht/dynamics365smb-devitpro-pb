---
title: "Record.TransferFields(var Record [, Boolean]) Method"
description: "Copies all matching fields in one record to another record."
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
# Record.TransferFields(var Record [, Boolean]) Method
> **Version**: _Available or changed with runtime version 1.0._

Copies all matching fields in one record to another record.


## Syntax
```AL
 Record.TransferFields(var FromRecord: Record [, InitPrimaryKeyFields: Boolean])
```
## Parameters
*Record*  
&emsp;Type: [Record](record-data-type.md)  
An instance of the [Record](record-data-type.md) data type.  

*FromRecord*  
&emsp;Type: [Record](record-data-type.md)  
The record from which to copy.  

*[Optional] InitPrimaryKeyFields*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
Default: true
If this parameter is true and the records are in the same table, both the timestamp and the Primary Key fields of the destination record will be changed.
If this parameter is true and the records are not in the same table, then the Primary Key fields of the destination record will be changed but the timestamp of the destination record will not be changed.
If this parameter is false, then neither the timestamp nor the Primary Key fields of the destination record are changed.  



[//]: # (IMPORTANT: END>DO_NOT_EDIT)

## Remarks

The `TransferFields` method copies fields based on the field number on the fields. For each field in `Record` (the destination), the contents of the field that has the same field number in `FromRecord` (the source) will be copied, if such a field exists.

The fields must have the *same data type* for the copying to succeed (text and code are convertible, other types are not). Enum fields are considered being the same data type even on different enum types. There must be room for the actual length of the contents of the field to be copied in the field to which it is to be copied. If any one of these conditions aren't fulfilled, a runtime error will occur.

> [!NOTE]
> When using `TransferFields` errors will only occur if there's a mismatch between fields originating from the *same extension*. Fields from different apps don't cause `TransferFields` to fail due to type mismatches. This behavior is to ensure that the addition of new extensions doesn't disrupt the operation of existing code.

> [!NOTE]  
> Fields are assigned, such as `DestinationRecord.Field := SourceRecord.Field`, which won't call the OnValidate trigger on the destination field. To assist with validation when using the `TransferFields` method, the `TypeHelper` codeunit contains a `TransferFieldsWithValidate` method.

## See also

[Record data type](record-data-type.md)  
[Get started with AL](../../devenv-get-started.md)  
[Developing extensions](../../devenv-dev-overview.md)
