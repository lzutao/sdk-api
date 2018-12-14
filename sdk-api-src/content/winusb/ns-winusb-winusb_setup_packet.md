---
UID: NS:winusb._WINUSB_SETUP_PACKET
title: WINUSB_SETUP_PACKET
author: windows-sdk-content
description: The WINUSB_SETUP_PACKET structure describes a USB setup packet.
old-location: buses\winusb_setup_packet.htm
tech.root: usbref
ms.assetid: b2e6bebc-81c1-4f52-870d-43c72740f8e2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PWINUSB_SETUP_PACKET, PWINUSB_SETUP_PACKET, PWINUSB_SETUP_PACKET structure pointer [Buses], WINUSB_SETUP_PACKET, WINUSB_SETUP_PACKET structure [Buses], buses.winusb_setup_packet, usbstrct_8a7725be-7ee3-4715-8498-3168b011c2dd.xml, winusb/PWINUSB_SETUP_PACKET, winusb/WINUSB_SETUP_PACKET"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winusb.h
req.include-header: Winusbio.h
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
 - winusb.h
api_name:
 - WINUSB_SETUP_PACKET
product: Windows
targetos: Windows
req.typenames: WINUSB_SETUP_PACKET, *PWINUSB_SETUP_PACKET
req.redist: 
---

# WINUSB_SETUP_PACKET structure


## -description


The <b>WINUSB_SETUP_PACKE</b>T structure describes a USB setup packet.


## -struct-fields




### -field RequestType

The request type. The values that are assigned to this member are defined in Table 9.2 of section 9.3 of the Universal Serial Bus (USB) specification (www.usb.org). 


### -field Request

The device request. The values that are assigned to this member are defined in Table 9.3 of section 9.4 of the Universal Serial Bus (USB) specification.


### -field Value

The meaning of this member varies according to the request. For an explanation of this member, see the Universal Serial Bus (USB) specification.


### -field Index

The meaning of this member varies according to the request. For an explanation of this member, see the Universal Serial Bus (USB) specification.


### -field Length

The number of bytes to transfer.


## -remarks



Callers of the <a href="https://msdn.microsoft.com/2ae80c97-3a09-4e90-ae73-92b5caa5cf99">WinUsb_ControlTransfer</a> routine must pass in a <b>WINUSB_SETUP_PACKET</b> structure. 




## -see-also




<a href="https://msdn.microsoft.com/8ca7033d-6586-4c34-b940-67ddfbe21af9">USB Structures</a>



<a href="https://msdn.microsoft.com/2ae80c97-3a09-4e90-ae73-92b5caa5cf99">WinUsb_ControlTransfer</a>
 

 
