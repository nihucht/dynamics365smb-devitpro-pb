---
title: "Page.RunModal() Method"
description: "Creates, opens, and closes a page that you specify."
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
# Page.RunModal() Method
> **Version**: _Available or changed with runtime version 1.0._

Creates, opens, and closes a page that you specify. When a page is run modally, no input, such as a keyboard or mouse click, can occur except for objects on the modal page.


## Syntax
```AL
[Action := ]  Page.RunModal()
```
## Parameters
*Page*  
&emsp;Type: [Page](page-data-type.md)  
An instance of the [Page](page-data-type.md) data type.  

## Return Value
*[Optional] Action*  
&emsp;Type: [Action](../action/action-option.md)  
Specifies what action the user took on the page.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)

Specifies what action the user took on the page. The following table shows the possible return values for the different user actions.

<!--NAV
In some cases, the actions for the return values are different when the page displays in the [!INCLUDE[d365fin_web_md](../includes/d365fin_web_md.md)] than in the [!INCLUDE[nav_windows](../includes/nav_windows_md.md)].
-->

|  Return value  |  Description  |  
|----------------|---------------|  
|OK|To close the page window, the user does one of the following:<br /><br /> -   Chooses the **Close** button.<br />-   Chooses the **X** button when there is no **Cancel** button on the window.|  
|Cancel|To close the page window, the user does one of the following:<br /><br /> -   Chooses the **Cancel** button.<br />-   Chooses the **X** button when there is a **Cancel** button on the window.|  
|LookupOK|To close a lookup window, the user chooses the **OK** button.|  
|LookupCancel|To close a lookup window, the user chooses the **Cancel** button.|  
|Yes|To close a confirmation window, the user selects **Yes**.|  
|No|To close a confirmation window, the user does one of the following:<br /><br /> -   Chooses the **No** button.<br />-   Chooses the **X** button.|  
|RunObject|The user selected an option that ran another object.|  
|RunSystem|The user selected an option that ran an external program.|  

## Remarks

If you know the specific page that you want to run when you are designing your application, then you can create a Page variable, set the Subtype of the variable to a specific page, and then use this method or the [Run Method \(Page\)](page-run--method.md).  

If you do not know the specific page that you want to run, then use the [Run Method \(Page\)](page-run--method.md) or the **RunModal Method \(Page\)** and specify the page in the *Number* parameter.  

After you define the page variable, you can use it before and after you run the page. If you use the [Run Method \(Page\)](page-run--method.md), then you can only use the variable before you run the page.  

## Example

This example shows how to use this method. Assume that the *SomePage* variable has been defined as `Page 1`.  

```al
Clear(SomePage);  
SomePage.XXX; // Any user-defined method  
SomePage.SetTableView(MyRecord);  
SomePage.SetRecord(MyRecord);  
if SomePage.RunModal = Action::LookupOK then  
  SomePage.GetRecord(MyRecord)...  
```  

> [!NOTE]  
> This code example includes the [Clear Method](../system/system-clear-joker-method.md) to make sure that the variable has been cleared.  

## See Also
[Page Data Type](page-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)