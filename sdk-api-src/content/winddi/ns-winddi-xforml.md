---
UID: NS:winddi._XFORML
title: XFORML
author: windows-sdk-content
description: The FLOATOBJ_XFORM structure describes an arbitrary linear two-dimensional transform, such as for geometric wide lines.
old-location: display\floatobj_xform.htm
tech.root: display
ms.assetid: 0c58a0df-4a0a-46e2-90de-dc50b8077709
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPFLOATOBJ_XFORM, *PFLOATOBJ_XFORM, *PXFORML, FAR *LPFLOATOBJ_XFORM, FAR *LPFLOATOBJ_XFORM structure [Display Devices], FLOATOBJ_XFORM, FLOATOBJ_XFORM structure [Display Devices], PFLOATOBJ_XFORM, PFLOATOBJ_XFORM structure pointer [Display Devices], XFORML, display.floatobj_xform, grstrcts_a53b73a9-2233-4cdf-bc65-d7db00c3ec9b.xml, winddi/FAR *LPFLOATOBJ_XFORM, winddi/FLOATOBJ_XFORM, winddi/PFLOATOBJ_XFORM"
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
 - FLOATOBJ_XFORM
product: Windows
targetos: Windows
req.typenames: XFORML, *PXFORML
req.redist: 
---

# XFORML structure


## -description


The FLOATOBJ_XFORM structure describes an arbitrary linear two-dimensional transform, such as for geometric wide lines.


## -struct-fields




### -field eM11


### -field eM12


### -field eM21


### -field eM22

Are the four <a href="https://msdn.microsoft.com/5f8c401b-7487-4d75-a0a8-534fa7992a3d">FLOATOBJ</a> elements that comprise a 2x2 row-major matrix. The <b>eM11</b> member specifies the matrix element at row 1, column 1, the <b>eM12</b> member specifies the matrix element at row 1, column2, and so on.


### -field eDx


### -field eDy

Are the x- and y-translation components of the transform.


## -remarks



All elements are specified as <a href="https://msdn.microsoft.com/5f8c401b-7487-4d75-a0a8-534fa7992a3d">FLOATOBJ</a> values. The transform can be downloaded to the driver. Structure members can be operated on by the <b>FLOATOBJ_</b><i>Xxx</i> routines.




## -see-also




<a href="https://msdn.microsoft.com/5f8c401b-7487-4d75-a0a8-534fa7992a3d">FLOATOBJ</a>



<a href="https://msdn.microsoft.com/0a78663c-15c9-4fed-b758-fea0f2571971">XFORMOBJ_iGetXform</a>
 

 
