---
title: "XmlProcessingInstruction.SetData(Text) Method"
description: "Sets the content of the processing instruction, excluding the target."
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
# XmlProcessingInstruction.SetData(Text) Method
> **Version**: _Available or changed with runtime version 1.0._

Sets the content of the processing instruction, excluding the target.


## Syntax
```AL
[Ok := ]  XmlProcessingInstruction.SetData(Value: Text)
```
## Parameters
*XmlProcessingInstruction*  
&emsp;Type: [XmlProcessingInstruction](xmlprocessinginstruction-data-type.md)  
An instance of the [XmlProcessingInstruction](xmlprocessinginstruction-data-type.md) data type.  

*Value*  
&emsp;Type: [Text](../text/text-data-type.md)  
The new content of the processing instruction, excluding the target.  


## Return Value
*[Optional] Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the operation was successful; otherwise **false**.   If you omit this optional return value and the operation does not execute successfully, a runtime error will occur.  


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[XmlProcessingInstruction Data Type](xmlprocessinginstruction-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)