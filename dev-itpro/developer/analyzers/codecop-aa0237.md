---
title: "CodeCop Warning AA0237"
description: "Only temporary variable names must be prefixed with Temp."
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
# CodeCop Warning AA0237
The name of non-temporary variables must not be prefixed with Temp.

## Description
Only temporary variable names must be prefixed with Temp.

[//]: # (IMPORTANT: END>DO_NOT_EDIT)

## Reason for the rule
Temporary variables must be named with identifiers that abbreviate the word temporary, such as `temp`. This improves readability of the code. Therefore you should avoid using `temp` for other purposes.

## Bad code example
```AL
TempJobWIPBuffer : Record "Job WIP Buffer";
```

## Good code example
```AL
CopyOfJobWIPBuffer : Record "Job WIP Buffer";
```
 
## See Also  
[CodeCop Analyzer](codecop.md)  
[Get Started with AL](../devenv-get-started.md)  
[Developing Extensions](../devenv-dev-overview.md)  