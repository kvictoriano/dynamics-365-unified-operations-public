--- 
# required metadata 
 
title: Create POS permission groups
description: This topic explains how to create a POS permission group. 
author: scott-tucker
manager: AnnBe 
ms.date: 08/20/2019
ms.topic: business-process 
ms.prod:  
ms.service: dynamics-ax-applications 
ms.technology:  
 
# optional metadata 
 
ms.search.form: RetailPosPermissionGroup, HcmJob   
audience: Application User 
# ms.devlang:  
ms.reviewer: josaw
#ms.search.scope: Core, Operations 
# ms.tgt_pltfrm:  
# ms.custom:  
ms.search.region: Global
ms.search.industry: Retail
ms.author: scotttuc
ms.search.validFrom: 2016-06-30 
ms.dyn365.ops.version: Version 7.0.0 
---
# Create POS permission groups

[!include [banner](../includes/banner.md)]

This topic explains how to create a POS permission group. The demo data company used to create this task is USRT. This task is intended for the Commerce operations manager role.

1. In the navigation pane, go to **Modules > Retail and Commerce > Employees > Permission groups**.
2. Select **New**.
3. In the **POS permission group ID** field, type a value.
4. In the **Description** field, type a value.
5. Select **Yes** in the **View time clock entries** field. You can now enable or disable various permissions for your POS Permission group. For some permission you can set a value that will be used to evaluate if the POS user can perform the action. This task guide enables a few permission that might be given to a cashier.  
6. Select **Yes** in the **Allow create order** field.
7. Select **Yes** in the **Allow edit order** field.
8. Select **Yes** in the **Allow retrieve order** field.
9. Select **Yes** in the **Allow password change** field.
10. Select **Yes** in the **Allow blind close** field.
11. Select **Save**. After your changes are saved you need to run the Staff distribution schedule to push the changes to commerce channels. 
12. In the navigation pane, go to **Modules > Human resources > Jobs > Jobs**.
13. Next we will assign the POS permission group to a Job. In the list, find and select the desired record.
14. Select **Edit**.
15. Expand the **Job classification** section.
16. In the POS permission group field, enter or select a value. All Workers in Positions for this Job will use this POS permission group's settings unless the workers POS permissions have been overridden at their Position level.  
17. Select **Save**. After your changes are saved you need to run the Staff distribution schedule to push the changes to channels.  

