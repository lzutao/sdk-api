---
UID: NS:ddrawint._DD_DIRECTDRAW_GLOBAL
title: DD_DIRECTDRAW_GLOBAL
author: windows-sdk-content
description: The DD_DIRECTDRAW_GLOBAL structure contains driver information that describes the driver's device.
old-location: display\dd_directdraw_global.htm
tech.root: display
ms.assetid: a59f064b-48cf-4491-82cd-84f59467af87
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PDD_DIRECTDRAW_GLOBAL, DD_DIRECTDRAW_GLOBAL, DD_DIRECTDRAW_GLOBAL structure [Display Devices], ddrawint/DD_DIRECTDRAW_GLOBAL, ddstrcts_d176c3e5-1e8b-4ff6-ba62-2fcfc42a9e5b.xml, display.dd_directdraw_global"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ddrawint.h
req.include-header: Winddi.h
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
 - ddrawint.h
api_name:
 - DD_DIRECTDRAW_GLOBAL
product: Windows
targetos: Windows
req.typenames: "*PDD_DIRECTDRAW_GLOBAL, DD_DIRECTDRAW_GLOBAL"
req.redist: 
---

# DD_DIRECTDRAW_GLOBAL structure


## -description


The DD_DIRECTDRAW_GLOBAL structure contains driver information that describes the driver's device. 


## -struct-fields




### -field dhpdev

Handle to the driver's private <a href="https://msdn.microsoft.com/139a10e9-203b-499b-9291-8537eae9189c">PDEV</a>.


### -field dwReserved1

Reserved for use by the display driver.


### -field dwReserved2

Reserved for use by the display driver.


### -field lpDDVideoPortCaps

Points to an array of one or more <a href="https://msdn.microsoft.com/ea85f189-7308-48ad-b159-1809749f8183">DDVIDEOPORTCAPS</a> structures in which the driver should describe the DirectDraw <a href="https://msdn.microsoft.com/a1de1905-09f3-4689-ace9-06690a1f930a">video port extensions (VPE)</a> objects that it supports. The structures are allocated by DirectDraw; the number of structures is based on the value returned in the <b>dwMaxVideoPort</b> member of <a href="https://msdn.microsoft.com/529d60b5-658d-4d55-a599-fa35386c01a7">DDCORECAPS</a>.

This member is <b>NULL</b> when the driver does not implement the VPE.


## -remarks



DirectDraw allocates memory for this structure. Only one DD_DIRECTDRAW_GLOBAL definition exists per device. In a multimonitor system, each device has its own unique DD_DIRECTDRAW_GLOBAL structure. 

The <b>dwReserved1</b> and <b>dwReserved2</b> members can be used as required by the driver. For example, a driver might store pointers to internal data structures in these members.




## -see-also




<a href="https://msdn.microsoft.com/58e378b7-863a-46d4-91cb-904ed4e892a3">DD_DIRECTDRAW_LOCAL</a>
 

 
