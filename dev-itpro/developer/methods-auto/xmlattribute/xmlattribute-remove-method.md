---
title: "XmlAttribute.Remove() Method"
description: "Removes this node from its parent element."
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
# XmlAttribute.Remove() Method
> **Version**: _Available or changed with runtime version 1.0._

Removes this node from its parent element.


## Syntax
```AL
[Ok := ]  XmlAttribute.Remove()
```
## Parameters
*XmlAttribute*  
&emsp;Type: [XmlAttribute](xmlattribute-data-type.md)  
An instance of the [XmlAttribute](xmlattribute-data-type.md) data type.  

## Return Value
*[Optional] Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the operation was successful; otherwise **false**.   If you omit this optional return value and the operation does not execute successfully, a runtime error will occur.  


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[XmlAttribute Data Type](xmlattribute-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)