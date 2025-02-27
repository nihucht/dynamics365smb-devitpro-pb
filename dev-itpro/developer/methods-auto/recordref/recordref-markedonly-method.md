---
title: "RecordRef.MarkedOnly([Boolean]) Method"
description: "Activates a special filter."
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
# RecordRef.MarkedOnly([Boolean]) Method
> **Version**: _Available or changed with runtime version 5.3._

Activates a special filter. After you use this function, your view of the table includes only records marked by the Mark method (RecordRef).


## Syntax
```AL
[MarkedOnly := ]  RecordRef.MarkedOnly([MarkedOnly: Boolean])
```
> [!NOTE]
> This method can be invoked using property access syntax.
## Parameters
*RecordRef*  
&emsp;Type: [RecordRef](recordref-data-type.md)  
An instance of the [RecordRef](recordref-data-type.md) data type.  

*[Optional] MarkedOnly*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
Activates a special filter.  


## Return Value
*[Optional] MarkedOnly*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the special filter is being used; otherwise, **false**.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[RecordRef Data Type](recordref-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)