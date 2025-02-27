---
title: "OnBeforeValidateEvent (Table) Trigger Event"
description: "Executed before a field is validated when its value has been changed."
ms.author: solsen
ms.custom: na
ms.date: 03/11/2024
ms.tgt_pltfrm: na
ms.topic: reference
author: SusanneWindfeldPedersen
---
[//]: # (START>DO_NOT_EDIT)
[//]: # (IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT.)
[//]: # (Any modifications should be made in the .xml files in the ModernDev repo.)

# OnBeforeValidateEvent (Table) Trigger Event
> **Version**: _Available or changed with runtime version 1.0._

Executed before a field is validated when its value has been changed.


## Syntax
```AL
[EventSubscriber(ObjectType::Table, Database::<Table Name>, 'OnBeforeValidateEvent', '<Field Name>', <SkipOnMissingLicense>, <SkipOnMissingPermission>)]
local procedure MyProcedure(var Rec: Record; var xRec: Record; CurrFieldNo: Integer)
begin
    ...
end;
```

### Parameters

*Rec*  
&emsp;Type: [Record](../../../methods-auto/record/record-data-type.md)  
The table that raises the event.  

*xRec*  
&emsp;Type: [Record](../../../methods-auto/record/record-data-type.md)  
The table that raises the event.  

*CurrFieldNo*  
&emsp;Type: [Integer](../../../methods-auto/integer/integer-data-type.md)  
The number of the field that raises the event.  



[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also  
[Get Started with AL](../../../devenv-get-started.md)  
[Developing Extensions](../../../devenv-dev-overview.md)   