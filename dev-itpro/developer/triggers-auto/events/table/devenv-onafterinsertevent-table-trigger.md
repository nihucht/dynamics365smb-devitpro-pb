---
title: "OnAfterInsertEvent (Table) Trigger Event"
description: "Executed after a record is inserted in a table."
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

# OnAfterInsertEvent (Table) Trigger Event
> **Version**: _Available or changed with runtime version 1.0._

Executed after a record is inserted in a table.


## Syntax
```AL
[EventSubscriber(ObjectType::Table, Database::<Table Name>, 'OnAfterInsertEvent', '', <SkipOnMissingLicense>, <SkipOnMissingPermission>)]
local procedure MyProcedure(var Rec: Record; RunTrigger: Boolean)
begin
    ...
end;
```

### Parameters

*Rec*  
&emsp;Type: [Record](../../../methods-auto/record/record-data-type.md)  
The table that raises the event.  

*RunTrigger*  
&emsp;Type: [Boolean](../../../methods-auto/boolean/boolean-data-type.md)  
Specifies whether to execute the code in the event trigger when it is invoked. If this parameter is true, the code will be run. If this parameter is false, then the code is not run.  



[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also  
[Get Started with AL](../../../devenv-get-started.md)  
[Developing Extensions](../../../devenv-dev-overview.md)   