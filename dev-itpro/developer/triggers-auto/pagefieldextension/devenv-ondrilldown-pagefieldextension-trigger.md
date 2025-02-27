---
title: "OnDrillDown (Page Field Extension) Trigger"
description: "Overrides the default drill-down behavior defined in the table definition for the FlowField."
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

# OnDrillDown (Page Field Extension) Trigger
> **Version**: _Available or changed with runtime version 3.0._

Overrides the default drill-down behavior defined in the table definition for the FlowField.


## Syntax
```AL
trigger OnDrillDown()
begin
    ...
end;
```



[//]: # (IMPORTANT: END>DO_NOT_EDIT)

> [!NOTE]  
> The OnDrillDown trigger is not invoked on fields in a Repeater control<!--NAV in the [!INCLUDE[nav_web](../includes/nav_web_md.md)]-->.  

## Remarks 
The [DrillDown Property](../../properties/devenv-drilldown-property.md) must be set to **True** to enable the drill-down.

If there is an error in the trigger code, the drilldown is canceled. You can use this trigger to write to the database.  

This trigger overrides the [DrillDownPageID Property](../../properties/devenv-drilldownpageid-property.md) setting of the FlowField.  

## See Also  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)  
[OnDrillDown (Page Field) Trigger](../pagefield/devenv-ondrilldown-pagefield-trigger.md)
