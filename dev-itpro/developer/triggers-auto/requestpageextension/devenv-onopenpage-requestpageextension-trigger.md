---
title: "OnOpenPage (Request Page Extension) Trigger"
description: "Runs after a request page is initialized and run."
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

# OnOpenPage (Request Page Extension) Trigger
> **Version**: _Available or changed with runtime version 7.0._

Runs after a request page is initialized and run.


## Syntax
```AL
trigger OnOpenPage()
begin
    ...
end;
```



[//]: # (IMPORTANT: END>DO_NOT_EDIT)

## Remarks

This trigger is executed after the [OnInit Trigger](../page/devenv-oninit-page-trigger.md).  

You use the **OnOpenPage** trigger to change dynamic properties, including those which can only be changed when the page is opened, such as the [Visible Property](../../properties/devenv-visible-property.md). You can also write to the database from the trigger.  

The **OnOpenPage** trigger is the only trigger that can toggle the [Visible Property](../../properties/devenv-visible-property.md) and the property can only be toggled on columns. 

If an error occurs in the trigger execution, then the page closes.  

> [!NOTE]  
> If you use the [LockTable Record](../../methods-auto/record/record-locktable-method.md) in the OnOpenPage trigger, then the table lock will be released when the trigger completes execution and not when the user closes the page.  

> [!NOTE]  
> The **OnOpenPage** trigger does not support calls to control add-in methods and properties because the trigger is invoked before the page is instantiated. <!-- For more information see, [Exposing Methods and Properties in a Windows Client Control Add-in](exposing-methods-and-properties-in-a-windows-client-pagefield-add-in.md).-->

## See Also  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)  
[OnOpenPage (Page) Trigger](../page/devenv-onopenpage-page-trigger.md)  
[OnOpenPage (Request Page) Trigger](../requestpage/devenv-onopenpage-requestpage-trigger.md)  
[OnOpenPage (Page Extension) Trigger](../pageextension/devenv-onopenpage-pageextension-trigger.md)
