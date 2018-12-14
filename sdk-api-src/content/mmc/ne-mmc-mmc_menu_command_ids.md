---
UID: NE:mmc._MMC_MENU_COMMAND_IDS
title: MMC_MENU_COMMAND_IDS
author: windows-sdk-content
description: The MMC_MENU_COMMAND_IDS enumeration defines the Command Identifiers that are reserved by MMC.
old-location: mmc\mmc_menu_command_ids.htm
tech.root: mmc
ms.assetid: 4e3e4289-ced2-4d94-af5e-e01a3d7afa32
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MMCC_STANDARD_VIEW_SELECT, MMC_MENU_COMMAND_IDS, MMC_MENU_COMMAND_IDS enumeration [MMC], _slate_mmc_menu_command_ids, mmc.mmc_menu_command_ids, mmc/MMCC_STANDARD_VIEW_SELECT, mmc/MMC_MENU_COMMAND_IDS
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: mmc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Mmc.h
api_name:
 - MMC_MENU_COMMAND_IDS
product: Windows
targetos: Windows
req.typenames: MMC_MENU_COMMAND_IDS
req.redist: 
---

# MMC_MENU_COMMAND_IDS enumeration


## -description


The 
<b>MMC_MENU_COMMAND_IDS</b> enumeration defines the Command Identifiers that are reserved by MMC.


## -enum-fields




### -field MMCC_STANDARD_VIEW_SELECT

Sent to a snap-in's 
<a href="https://msdn.microsoft.com/ee91a737-c6b4-48a1-88a2-57bef3730f5e">IExtendContextMenu::Command</a> method when the user switches from a custom result view to the standard list view.


## -remarks



Typically, a snap-in's 
<a href="https://msdn.microsoft.com/ee91a737-c6b4-48a1-88a2-57bef3730f5e">IExtendContextMenu::Command</a> method is called only when one of its own menu items is selected. The MMCC_* codes are sent when a built-in menu item is selected and the snap-in must be notified about the selection. Other MMCC_* codes can be added later.

MMCC_STANDARD_VIEW_SELECT notifies the snap-in that the custom view is going away and that the snap-in can do any necessary clean-up. The next time the snap-in's 
<a href="https://msdn.microsoft.com/d2575f79-d646-41b5-84a5-768402cfb826">IComponent::GetResultViewType</a> method is called, the snap-in should return S_FALSE to indicate that the default list view should be used.


