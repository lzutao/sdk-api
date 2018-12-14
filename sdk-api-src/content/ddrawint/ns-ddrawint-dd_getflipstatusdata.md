---
UID: NS:ddrawint._DD_GETFLIPSTATUSDATA
title: DD_GETFLIPSTATUSDATA
author: windows-sdk-content
description: The DD_GETFLIPSTATUSDATA structure returns the flip status information.
old-location: display\dd_getflipstatusdata.htm
tech.root: display
ms.assetid: da3b90e0-1a60-434b-966c-a7ebabff33ee
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PDD_GETFLIPSTATUSDATA, DD_GETFLIPSTATUSDATA, DD_GETFLIPSTATUSDATA structure [Display Devices], ddrawint/DD_GETFLIPSTATUSDATA, ddstrcts_03291da8-7881-46a2-8b11-291124a5732d.xml, display.dd_getflipstatusdata"
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
 - DD_GETFLIPSTATUSDATA
product: Windows
targetos: Windows
req.typenames: "*PDD_GETFLIPSTATUSDATA, DD_GETFLIPSTATUSDATA"
req.redist: 
---

# DD_GETFLIPSTATUSDATA structure


## -description


The DD_GETFLIPSTATUSDATA structure returns the flip status information.


## -struct-fields




### -field lpDD

Points to a <a href="https://msdn.microsoft.com/a59f064b-48cf-4491-82cd-84f59467af87">DD_DIRECTDRAW_GLOBAL</a> structure that describes the driver's device.


### -field lpDDSurface

Points to a <a href="https://msdn.microsoft.com/45a41cec-0257-4e26-809d-c2fc4c247328">DD_SURFACE_LOCAL</a> structure that describes the surface whose flip status is being queried.


### -field dwFlags

Specifies the flip status being requested. This member can be one of the following values:

<table>
<tr>
<th>Flag</th>
<th>Meaning</th>
</tr>
<tr>
<td>
DDGFS_CANFLIP

</td>
<td>
Queries whether the driver can currently perform a flip.

</td>
</tr>
<tr>
<td>
DDGFS_ISFLIPDONE

</td>
<td>
Queries whether the driver has finished the last flip.

</td>
</tr>
</table>
 


### -field ddRVal

Specifies the location in which the driver writes the return value of the <a href="https://msdn.microsoft.com/ec556891-e091-4c52-a155-cb6ba8011f71">DdGetFlipStatus</a> callback. A return code of DD_OK indicates success. For more information, see <a href="https://msdn.microsoft.com/da4cc7d7-6826-48aa-96c6-004e31fc3e3e">Return Values for DirectDraw</a>.


### -field GetFlipStatus

Used by the Microsoft DirectDraw API and should not be filled in by the driver.


## -see-also




<a href="https://msdn.microsoft.com/ec556891-e091-4c52-a155-cb6ba8011f71">DdGetFlipStatus</a>
 

 
