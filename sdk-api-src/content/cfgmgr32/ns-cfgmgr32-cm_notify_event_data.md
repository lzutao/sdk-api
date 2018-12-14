---
UID: NS:cfgmgr32._CM_NOTIFY_EVENT_DATA
title: CM_NOTIFY_EVENT_DATA
author: windows-sdk-content
description: This is a device notification event data structure.
old-location: devinst\cm_notify_event_data.htm
tech.root: devinst
ms.assetid: 61bd4ea3-9910-4feb-a330-3e0bcdac1ce2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCM_NOTIFY_EVENT_DATA, CM_NOTIFY_EVENT_DATA, CM_NOTIFY_EVENT_DATA structure [Device and Driver Installation], PCM_NOTIFY_EVENT_DATA, PCM_NOTIFY_EVENT_DATA structure pointer [Device and Driver Installation], cfgmgr32/CM_NOTIFY_EVENT_DATA, cfgmgr32/PCM_NOTIFY_EVENT_DATA, devinst.cm_notify_event_data"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: cfgmgr32.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - Cfgmgr32.h
api_name:
 - CM_NOTIFY_EVENT_DATA
product: Windows
targetos: Windows
req.typenames: CM_NOTIFY_EVENT_DATA, *PCM_NOTIFY_EVENT_DATA
req.redist: 
---

# CM_NOTIFY_EVENT_DATA structure


## -description


This is a device notification event data structure.


## -struct-fields




### -field FilterType

The <b>CM_NOTIFY_FILTER_TYPE</b> from the <a href="https://msdn.microsoft.com/8B6CC440-7B41-4382-9917-6833031D5E1B">CM_NOTIFY_FILTER</a> structure that was used in the registration that generated this notification event data.


### -field Reserved

Reserved.  Must be 0.


### -field u

A union that contains information about the notification event data.    To determine which member of the union to examine, check the <b>FilterType</b> of the event data.


### -field u.DeviceInterface

Examine this part of the union when the <b>FilterType</b> is <b>CM_NOTIFY_FILTER_TYPE_DEVICEINTERFACE</b>.


### -field u.DeviceInterface.ClassGuid

The GUID of the device interface class for the device interface to which the notification event data pertains.


### -field u.DeviceInterface.SymbolicLink

The symbolic link path of the device interface to which the notification event data pertains.


### -field u.DeviceHandle

Examine this part of the union when the <b>FilterType</b> is <b>CM_NOTIFY_FILTER_TYPE_DEVICEHANDLE</b> and the notification action is <b>CM_NOTIFY_ACTION_DEVICECUSTOMEVENT</b>.


### -field u.DeviceHandle.EventGuid

The GUID for the custom event.


### -field u.DeviceHandle.NameOffset

The offset of an optional string buffer.  Usage depends on the contract for the <b>EventGuid</b>.


### -field u.DeviceHandle.DataSize

The number of bytes that can be read from the <b>Data</b> member.


### -field u.DeviceHandle.Data

Optional binary data.  Usage depends on the contract for the <b>EventGuid</b>.


### -field u.DeviceInstance

Examine this part of the union when the <b>FilterType</b> is <b>CM_NOTIFY_FILTER_TYPE_DEVICEINSTANCE</b>.


### -field u.DeviceInstance.InstanceId

The device instance ID of the device to which the notification event data pertains.


## -remarks



The notification callback supplied to <a href="https://msdn.microsoft.com/15847F9C-9F2A-453F-9EF8-0AF63CFF93C9">CM_Register_Notification</a> receives a pointer to a structure of type <b>CM_NOTIFY_EVENT_DATA</b> in the callback's <i>EventData</i> parameter.




## -see-also




<a href="https://msdn.microsoft.com/15847F9C-9F2A-453F-9EF8-0AF63CFF93C9">CM_Register_Notification</a>
 

 
