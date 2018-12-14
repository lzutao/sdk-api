---
UID: NS:winddi._BRUSHOBJ
title: BRUSHOBJ
author: windows-sdk-content
description: The BRUSHOBJ structure contains three public members that describe a brush object.
old-location: display\brushobj.htm
tech.root: display
ms.assetid: 81216bee-d13f-4880-a839-337a247a6c82
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BRUSHOBJ, BRUSHOBJ structure [Display Devices], display.brushobj, grstrcts_eb8de3ab-7f42-4f7b-b4bd-7c3c739e52ed.xml, winddi/BRUSHOBJ
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winddi.h
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
 - winddi.h
api_name:
 - BRUSHOBJ
product: Windows
targetos: Windows
req.typenames: BRUSHOBJ
req.redist: 
---

# BRUSHOBJ structure


## -description


The <b>BRUSHOBJ</b> structure contains three public members that describe a brush object. 


## -struct-fields




### -field iSolidColor

Specifies the color index of a solid brush. This index has been translated to the target surface's palette. Drawing can proceed without realization of the brush. A value of 0xFFFFFFFF indicates that a nonsolid brush must be realized.


### -field pvRbrush

Pointer to the driver's realized brush.


### -field flColorType

Specifies an FLONG value containing flags that describe this brush object. This member can be a combination of any of the following values (only one of BR_HOST_ICM and BR_DEVICE_ICM can be set):

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td>
BR_CMYKCOLOR

</td>
<td>
When this bit is set, <b>iSolidColor</b> contains a 32-bit <a href="https://msdn.microsoft.com/ac439eb8-b491-4215-877d-5ee177fbdb39">CMYK</a> color value. Otherwise, <b>iSolidColor</b> contains a palette index or 0xFFFFFFFF.

</td>
</tr>
<tr>
<td>
BR_DEVICE_ICM

</td>
<td>
The driver performs image color management for the brush color.

</td>
</tr>
<tr>
<td>
BR_HOST_ICM

</td>
<td>
The driver need not perform image color management for the brush color because GDI (or the calling application) is responsible.

</td>
</tr>
</table>
 


## -remarks



Drivers can call <i>BRUSHOBJ_Xxx</i> service routines to realize brushes or to find previously realized brushes.

If the <b>iSolidColor</b> member is 0xFFFFFFFF or the <b>pvRbrush</b> member is <b>NULL</b>, the driver must call the <a href="https://msdn.microsoft.com/3f3e5acb-f984-4571-9555-f6b383ddb6a7">BRUSHOBJ_pvGetRbrush</a> function to realize the brush.

If neither BR_HOST_ICM or BR_DEVICE_ICM are set, ICM is not enabled in the graphics engine or in the driver.

For a description of the FLONG data type, see <a href="https://msdn.microsoft.com/2054aa16-6d86-4db3-8b16-4570b0374e23">GDI Data Types</a>. 




## -see-also




<a href="https://msdn.microsoft.com/a62544e5-f4b6-4544-8ec1-5a03f8bd3306">BRUSHOBJ_hGetColorTransform</a>



<b>BRUSHOBJ_pvGetRbrush</b>



<a href="https://msdn.microsoft.com/815844d7-930f-46c3-9403-c61cb2c8a992">BRUSHOBJ_ulGetBrushColor</a>
 

 
