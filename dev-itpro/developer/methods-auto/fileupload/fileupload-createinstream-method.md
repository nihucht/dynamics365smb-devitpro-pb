---
title: "FileUpload.CreateInStream(InStream, TextEncoding) Method"
description: "Creates an InStream object for a file."
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
# FileUpload.CreateInStream(InStream, TextEncoding) Method
> **Version**: _Available or changed with runtime version 13.0._

Creates an InStream object for a file. This enables you to import or read data from the file.


## Syntax
```AL
 FileUpload.CreateInStream(InStream: InStream, Encoding: TextEncoding)
```
## Parameters
*FileUpload*  
&emsp;Type: [FileUpload](fileupload-data-type.md)  
An instance of the [FileUpload](fileupload-data-type.md) data type.  

*InStream*  
&emsp;Type: [InStream](../instream/instream-data-type.md)  
The InStream object type that has been created.  

*Encoding*  
&emsp;Type: [TextEncoding](../textencoding/textencoding-option.md)  
The encoding that will be used by the stream. The default encoding is MSDos.  



[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[FileUpload Data Type](fileupload-data-type.md)  
[Getting Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)