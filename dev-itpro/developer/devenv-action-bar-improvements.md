---
title: Action bar improvements
description: Introducing the modern action bar in Dynamics 365 Business Central
author: jacobwj
ms.author: solsen
ms.reviewer: jswymer
ms.topic: conceptual
ms.date: 03/08/2024
ms.custom: bap-template
---

# Action bar improvements

With [!INCLUDE [prod_short](includes/prod_short.md)] 2024 release wave 1, we are making the modern action bar available and turned on for all users. Since its introduction in release wave 2, 2022, the modern action bar has been the default for *new* customers and is now becoming the default for *all* customers upgrading to release wave 1, 2024.

Users who have already been using the modern action bar will notice a few additional optimizations in its newest version, such as a more compact representation of Search and Analysis Mode, and the introduction of Microsoft Copilot!

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RW1jUai]

Users who have *not* been using the modern action bar with earlier releases of [!INCLUDE [prod_short](includes/prod_short.md)] will experience that the action bar looks different to what they were used to, and that some of their routines can need adjustment. The reason is that the modern action bar places some actions differently compared to the earlier action bar (now known as the **legacy action bar**) to give more prominence to important actions and reduce the numbers of clicks to access them.

## Split buttons enhance productivity

*Split buttons* are one of the new experiences in the modern action bar. Split buttons are well-known from other Microsoft products as a combination of a button and a menu and are introduced in cases where a common action has related actions with similar effects. This type of control gives quick one-click reach to the first action in a menu via the left button part and access to the related actions via the right dropdown part. 

For instance, on document pages that have **Post** and **Release** actions, these are now presented as split buttons. This provides better discoverability and one-click access to these often-used actions. For example, a new split button is created for the actions **Correct**, **Cancel**, and **Create** corrective credit memo. This provides one-click access to Correct, which is the most often used among the three. 

## Action tabs open by default

On document, card, worksheet, and listplus pages, the Process tab is renamed to **Home**, which better aligns with the ribbon terminology that users see in other Microsoft products. 

With document, card, worksheet, and listplus pages that have actions in the Home/Process group, the modern action bar starts in the pinned and opened state. This helps discovering relevant actions in the action bar and provides one-click reach to actions, without first pinning the action bar manually. With document pages that have a Lines subpage, or any other page having a subpage, the subpage's actions are now visible right away, without opening **More options**.

## Legacy action bar

While the majority of users are confident with split buttons, and likely know the concept from other software packages, in the rare cases where split buttons or some of the other modern action bar improvements are causing problems for a user, we provide a new personalization option to use the legacy action bar instead.

The Legacy Action Bar toggle is available in users' **My settings** page and reverts the action bar for individual users to the earlier appearance before the modern action bar. Note that we recommend using the modern action bar for the best productivity and that future releases of [!INCLUDE [prod_short](includes/prod_short.md)] may not provide the legacy action bar option.

## See also

[Actions in AL](devenv-actions-overview.md)  
[Adding Actions to a Page](devenv-adding-actions-to-a-page.md)  
[Actions in the User Interface](devenv-actions-user-interface.md)  
[How to Promote Actions](devenv-promoted-actions.md)  
[Organizing Promoted Actions](devenv-organizing-promoted-actions.md)  
[Common Promoted Action Groups](devenv-common-promoted-action-groups.md)  
[Action Bar Improvements](devenv-action-bar-improvements.md)  
[Behavioral Changes for Promoted Actions](devenv-promoted-actions-behavioral-changes.md)  
