---
title: "Guid Data Type"
description: "Represents a 16 byte binary data type."
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
# Guid Data Type
> **Version**: _Available or changed with runtime version 1.0._

Represents a 16 byte binary data type. This data type is used for the global identification of objects, programs, records, and so on. The important property of a GUID is that each value is globally unique. The value is generated by an algorithm, developed by Microsoft, which assures this uniqueness.




[//]: # (IMPORTANT: END>DO_NOT_EDIT)

The GUID is a 16-byte binary data type that can be logically grouped into the following subgroups:  
  
4byte-2byte-2byte-2byte-6byte.  
  
The standard textual representation is {12345678-1234-1234-1234-1234567890AB}.  
  
The virtual table OLE Control (2000000042) does not use the GUID data type. It uses a textual representation of the GUID in a text field instead. It is easier to make operations and references to this text field using the GUID data type than it is using the textual representation. The GUID data type is compatible with the existing textual representation.  
  
The GUID data type is useful when you want to uniquely identify some data, so that it can be exchanged with external applications. For example, if you want to transfer an item catalog to an external application, you add a GUID field to the record in the table and use this as the primary reference when you communicate with the external application.  
  
## Compatibility

You can assign and compare the Text data type and the GUID data type. Assigning a Text to a GUID can be done as follows:  
  
```al
MyTableRec.MyGuid  :=  MyTableRec.MyText;  
```  

The supported formats of `MyText` are:

`'11111111-1111-1111-1111-111111111111'`
`'{22222222-2222-2222-2222-222222222222}'`

## Methods and properties

The following AL methods can be used with the GUID data type:  
  
```al
Guid := CreateGUID();  
```  
  
This method creates a new unique GUID value. The value can then be assigned to a field of the GUID data type or of the Text data type.  
  
```al 
Ok := IsNullGUID(Guid);  
```  
  
This method is a convenient way to check if a value has already been assigned to a GUID. A NULL GUID \(consisting only of zeroes\) is valid, but should never be used for reference purposes.  
  
A NULL GUID is valid but is not useful in a table. Therefore, the **AutoSplitKey** property is implemented for the GUID data type when it is used in a page. When GUID is selected as a primary key, **AutoSplitKey** is enabled for the page, and the GUID value remains NULL. When you create a new record, a valid GUID is created and assigned automatically.  
  
The [CreateGUID method](../system/system-createguid-method.md) and [IsNullGUID method](../system/system-IsNullGUID-method.md) methods are available in the AL Symbol Menu under SYSTEM, Variables.  
  
CreateGUID takes no arguments and returns a valid 16-byte GUID value. If the result is assigned to a TEXT variable or field, the value is converted to a string and follows the syntax explained earlier. The algorithm that generates the new GUID value uses Microsoft's CoCreateGuid method.  
  
IsNullGUID takes a GUID value as a required argument and returns True/False depending on whether the GUID value is NULL. This method does not accept a Text value as an argument.  
  
**AutoSplitKey** is a property, not a method and can be applied to pages. If you have defined a GUID field as part of the primary key, the **AutoSplitKey** property automatically generates a new valid GUID value. When a new record is created and the GUID field is left as NULL, the **AutoSplitKey** property ensures that a valid GUID value is automatically inserted into the field. If you then enter a NULL GUID into this record, for example, by using the Clear method, this new NULL GUID value is not automatically replaced by the **AutoSplitKey** property. The **AutoSplitKey** property only applies to new records.  
  
## Format  
The GUID value can also be represented as text. You can use the standard AL methods [Format](../system/system-format-joker-integer-string-method.md) and [Evaluate](../system/system-evaluate-method.md) to convert from GUID values to Text values. If you do not use the correct format when you edit a GUID value in its textual format, the following error message is displayed:  
  
**Invalid Format of GUID string. The correct format of the GUID string is {CDEF7890-ABCD-1234-ABCD-1234567890AB} where 0-9, A-F symbolizes hexadecimal digits.**  

## See Also

[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)  