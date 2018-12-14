---
UID: NF:mmc.IExtendControlbar.ControlbarNotify
title: IExtendControlbar::ControlbarNotify
author: windows-sdk-content
description: The IExtendControlbar::ControlbarNotify method specifies the notification sent to the snap-in from the console as a result of user action.
old-location: mmc\iextendcontrolbar_controlbarnotify.htm
tech.root: mmc
ms.assetid: 124656df-5d12-4de1-9a71-ba080ef36611
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ControlbarNotify, ControlbarNotify method [MMC], ControlbarNotify method [MMC],IExtendControlbar interface, IExtendControlbar interface [MMC],ControlbarNotify method, IExtendControlbar.ControlbarNotify, IExtendControlbar::ControlbarNotify, MMCN_BTN_CLICK, MMCN_DESELECT_ALL, MMCN_MENU_BTNCLICK, MMCN_SELECT, _slate_iextendcontrolbar_controlbarnotify, mmc.iextendcontrolbar_controlbarnotify, mmc/IExtendControlbar::ControlbarNotify
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
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
 - COM
api_location:
 - Mmc.h
api_name:
 - IExtendControlbar.ControlbarNotify
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IExtendControlbar::ControlbarNotify


## -description


The <b>IExtendControlbar::ControlbarNotify</b> method specifies the notification sent to the snap-in from the console as a result of user action.


## -parameters




### -param event [in]

A value that specifies one of the following:



#### MMCN_BTN_CLICK

A button on the toolbar was clicked.



#### MMCN_DESELECT_ALL

All items of a virtual list are deselected.



#### MMCN_SELECT

An item was selected and the snap-in should update the toolbar options.



#### MMCN_MENU_BTNCLICK

A menu button on the toolbar is clicked.


### -param arg [in]

Depends on the event parameter. For more information, see 
<a href="https://msdn.microsoft.com/8d5aa622-5668-495a-bc3a-25b863fbcb81">MMC Notifications</a>.


### -param param [in]

Depends on the event parameter. For more information, see 
<a href="https://msdn.microsoft.com/8d5aa622-5668-495a-bc3a-25b863fbcb81">MMC Notifications</a>.


## -returns



This method can return one of these values.




## -remarks



For more information, see the individual notifications. The snap-in should return S_FALSE for any notification it does not handle.




## -see-also




<a href="https://msdn.microsoft.com/cf9c9fe9-f58f-47f0-9051-86a514df0c6d">IToolbar</a>
 

 
