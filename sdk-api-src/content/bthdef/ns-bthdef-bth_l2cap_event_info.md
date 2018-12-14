---
UID: NS:bthdef._BTH_L2CAP_EVENT_INFO
title: BTH_L2CAP_EVENT_INFO
author: windows-sdk-content
description: Contains data about events associated with an L2CAP channel.
old-location: bluetooth\bth_l2cap_event_info.htm
tech.root: Bluetooth
ms.assetid: fd16514c-7a7e-4da4-b506-71cb66ed1983
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PBTH_L2CAP_EVENT_INFO, *PBTH_L2CAP_EVENT_INFO structure [Bluetooth], BTH_L2CAP_EVENT_INFO, BTH_L2CAP_EVENT_INFO structure [Bluetooth], bluetooth.bth_l2cap_event_info, bthdef/*PBTH_L2CAP_EVENT_INFO, bthdef/BTH_L2CAP_EVENT_INFO"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: bthdef.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: None supported
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
 - Bthdef.h
api_name:
 - BTH_L2CAP_EVENT_INFO
product: Windows
targetos: Windows
req.typenames: BTH_L2CAP_EVENT_INFO, *PBTH_L2CAP_EVENT_INFO
req.redist: 
---

# BTH_L2CAP_EVENT_INFO structure


## -description


The <b>BTH_L2CAP_EVENT_INFO</b> structure contains data about events associated with an L2CAP channel.


## -struct-fields




### -field bthAddress

Remote radio address with which the L2CAP event is associated, in the form of a <a href="https://msdn.microsoft.com/81dd4925-7f0a-468f-b706-244ce99e91df">BTH_ADDR</a> structure.


### -field psm

Channel number established or terminated.


### -field connected

Status of the connection. If nonzero, the channel has been established. If zero, the channel has been terminated.


### -field initiated

Provides connection information. If nonzero, the local radio initiated the L2CAP connection.  If zero,  the remote Bluetooth device initiated the L2CAP connection.  If <b>connected</b> is zero,  this member is undefined and  not applicable.


## -remarks



Notifications for a destroyed channel are only to be sent for channels that have been successfully established.




## -see-also




<a href="https://msdn.microsoft.com/81dd4925-7f0a-468f-b706-244ce99e91df">BTH_ADDR</a>



<a href="https://msdn.microsoft.com/ca28c9cd-a271-48fa-901c-e99e063854d5">Bluetooth and WM_DEVICECHANGE
			 Messages</a>
 

 
