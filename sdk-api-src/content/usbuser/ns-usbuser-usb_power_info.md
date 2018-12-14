---
UID: NS:usbuser._USB_POWER_INFO
title: USB_POWER_INFO
author: windows-sdk-content
description: The USB_POWER_INFO structure is used with the IOCTL_USB_USER_REQUEST I/O control request to retrieve device power state that the host controller power policy specifies for the indicated system power state.
old-location: buses\usb_power_info.htm
tech.root: usbref
ms.assetid: b4f35d7e-b0e3-44d9-8e41-1752cb0af5ef
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PUSB_POWER_INFO, PUSB_POWER_INFO, PUSB_POWER_INFO structure pointer [Buses], USB_POWER_INFO, USB_POWER_INFO structure [Buses], buses.usb_power_info, usbstrct_95ba66ea-20ee-4e05-8294-3b3bd06f7116.xml, usbuser/PUSB_POWER_INFO, usbuser/USB_POWER_INFO"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: usbuser.h
req.include-header: Usbuser.h
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
 - usbuser.h
api_name:
 - USB_POWER_INFO
product: Windows
targetos: Windows
req.typenames: USB_POWER_INFO, *PUSB_POWER_INFO
req.redist: 
---

# USB_POWER_INFO structure


## -description


The <b>USB_POWER_INFO</b> structure is used with the <a href="https://msdn.microsoft.com/6aba5cf4-a9fa-4d10-a212-acc79e00fa9b">IOCTL_USB_USER_REQUEST</a> I/O control request to retrieve device power state that the host controller power policy specifies for the indicated system power state.


## -struct-fields




### -field SystemState

On input, a <a href="https://msdn.microsoft.com/2f64bd5b-507c-4824-b50c-dbc228e8671a">WDMUSB_POWER_STATE</a>-type enumerator value that specifies the system power state.


### -field HcDevicePowerState

On output, an <a href="https://msdn.microsoft.com/2f64bd5b-507c-4824-b50c-dbc228e8671a">WDMUSB_POWER_STATE</a>-type enumerator value that specifies the device power state of the host controller.


### -field HcDeviceWake

On output, a <a href="https://msdn.microsoft.com/2f64bd5b-507c-4824-b50c-dbc228e8671a">WDMUSB_POWER_STATE</a>-type enumerator value that specifies whether the host controller is in a wake state.


### -field HcSystemWake

On output, a <a href="https://msdn.microsoft.com/2f64bd5b-507c-4824-b50c-dbc228e8671a">WDMUSB_POWER_STATE</a>-type enumerator value that specifies whether the host controller can wake the system.


### -field RhDevicePowerState

On output, a <a href="https://msdn.microsoft.com/2f64bd5b-507c-4824-b50c-dbc228e8671a">WDMUSB_POWER_STATE</a>-type enumerator value that specifies the device power state of the root hub.


### -field RhDeviceWake

On output, a <a href="https://msdn.microsoft.com/2f64bd5b-507c-4824-b50c-dbc228e8671a">WDMUSB_POWER_STATE</a>-type enumerator value that specifies whether the root hub is in a wake state.


### -field RhSystemWake

On output, a <a href="https://msdn.microsoft.com/2f64bd5b-507c-4824-b50c-dbc228e8671a">WDMUSB_POWER_STATE</a>-type enumerator value that specifies whether the root hub can wake the system.


### -field LastSystemSleepState

On output, a <a href="https://msdn.microsoft.com/2f64bd5b-507c-4824-b50c-dbc228e8671a">WDMUSB_POWER_STATE</a>-type enumerator value that specifies the last system sleep state.


### -field CanWakeup

A Boolean value that indicates whether the host controller device can wake up the system from the specified system power state. If <b>TRUE</b>, the host controller device can wake up the system. If <b>FALSE</b>, the host controller cannot wake up the system.


### -field IsPowered

A Boolean value that indicates whether the host controller is powered when in the specified system power state. If <b>TRUE</b>, the host controller is powered. If <b>FALSE</b>, the host controller is not powered.


## -remarks



The <b>USB_POWER_INFO</b> structure is used with the USBUSER_GET_POWER_STATE_MAP user-mode request. For more information about this request, see <a href="https://msdn.microsoft.com/6aba5cf4-a9fa-4d10-a212-acc79e00fa9b">IOCTL_USB_USER_REQUEST</a>.




## -see-also




<a href="https://msdn.microsoft.com/6aba5cf4-a9fa-4d10-a212-acc79e00fa9b">IOCTL_USB_USER_REQUEST</a>



<a href="https://msdn.microsoft.com/8ca7033d-6586-4c34-b940-67ddfbe21af9">USB Structures</a>
 

 
