---
UID: NS:ddrawint._DDMOCOMPBUFFERINFO
title: DDMOCOMPBUFFERINFO
author: windows-sdk-content
description: The DDMOCOMPBUFFERINFO structure contains the macro block information required to render a frame and passes this information to the DD_RENDERMOCOMPDATA structure.
old-location: display\ddmocompbufferinfo.htm
tech.root: display
ms.assetid: e039f85e-868f-4673-bbaa-9165bd760e9d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPDDMOCOMPBUFFERINFO, DDMOCOMPBUFFERINFO, DDMOCOMPBUFFERINFO structure [Display Devices], LPDDMOCOMPBUFFERINFO, LPDDMOCOMPBUFFERINFO structure pointer [Display Devices], ddrawint/DDMOCOMPBUFFERINFO, ddrawint/LPDDMOCOMPBUFFERINFO, ddstrcts_8716da01-eda5-4102-b881-c2e368f0792a.xml, display.ddmocompbufferinfo"
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
 - DDMOCOMPBUFFERINFO
product: Windows
targetos: Windows
req.typenames: DDMOCOMPBUFFERINFO, *LPDDMOCOMPBUFFERINFO
req.redist: 
---

# DDMOCOMPBUFFERINFO structure


## -description


The DDMOCOMPBUFFERINFO structure contains the macro block information required to render a frame and passes this information to the <a href="https://msdn.microsoft.com/a890707f-b773-4b66-8817-68efdb8d47f8">DD_RENDERMOCOMPDATA</a> structure. 


## -struct-fields




### -field dwSize

Specifies the size in bytes of this DDMOCOMPBUFFERINFO structure.


### -field lpCompSurface

Points to a <a href="https://msdn.microsoft.com/45a41cec-0257-4e26-809d-c2fc4c247328">DD_SURFACE_LOCAL</a> structure that contains the compressed data. 


### -field dwDataOffset

Indicates the offset to the relevant data, in bytes, from the beginning of the buffer. This value does not allow for pitch.


### -field dwDataSize

Indicates the size of the relevant data in bytes. This value does not allow for pitch.


### -field lpPrivate

Used by Microsoft DirectDraw and should be ignored by the driver.


## -see-also




<a href="https://msdn.microsoft.com/a890707f-b773-4b66-8817-68efdb8d47f8">DD_RENDERMOCOMPDATA</a>



<a href="https://msdn.microsoft.com/45a41cec-0257-4e26-809d-c2fc4c247328">DD_SURFACE_LOCAL</a>
 

 
