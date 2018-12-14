---
UID: NS:amva._tag_AMVABeginFrameInfo
title: AMVABeginFrameInfo
author: windows-sdk-content
description: The AMVABeginFrameInfo structure contains information for the IAMVideoAccelerator::BeginFrame method.
old-location: dshow\amvabeginframeinfo.htm
tech.root: DirectShow
ms.assetid: 49af9094-86d5-4c11-b871-41f9984e0faf
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPAMVABeginFrameInfo, AMVABeginFrameInfo, AMVABeginFrameInfo structure [DirectShow], AMVABeginFrameInfoStructure, LPAMVABeginFrameInfo, LPAMVABeginFrameInfo structure pointer [DirectShow], amva/AMVABeginFrameInfo, amva/LPAMVABeginFrameInfo, dshow.amvabeginframeinfo"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: amva.h
req.include-header: Videoacc.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - amva.h
api_name:
 - AMVABeginFrameInfo
product: Windows
targetos: Windows
req.typenames: AMVABeginFrameInfo, *LPAMVABeginFrameInfo
req.redist: 
---

# AMVABeginFrameInfo structure


## -description


The <b>AMVABeginFrameInfo</b> structure contains information for the <a href="https://msdn.microsoft.com/en-us/library/Dd375997(v=VS.85).aspx">IAMVideoAccelerator::BeginFrame</a> method.


## -struct-fields




### -field dwDestSurfaceIndex

The zero-based index of the uncompressed destination surface. The number of uncompressed surfaces is specified in the <a href="https://msdn.microsoft.com/en-us/library/Dd375996(v=VS.85).aspx">IAMVideoAcceleratorNotify::SetUncompSurfacesInfo</a> method.


### -field pInputData

Pointer to a buffer that contains data for the video accelerator.

This buffer must contain a <b>WORD</b> value that is equal to the value of <b>dwDestSurfaceIndex</b>.


### -field dwSizeInputData

Size, in bytes, of the buffer that <b>pInputData</b> points to. The value must be 2.


### -field pOutputData

Pointer to a buffer that the video accelerator can write to.

This member must be <b>NULL</b>.


### -field dwSizeOutputData

Size, in bytes, of the buffer that <b>pOutputData</b> points to. The value must be zero.


## -remarks



The buffer pointed to by <b>pInputData</b> cannot contain pointer values, because their addresses will not be valid in kernel mode, where frame processing occurs.
      

The video accelerator might not use the same surface memory in two consecutive calls with the same frame index.
      Therefore, the decoder should not make any assumption about the initial contents of the frame.




## -see-also




<a href="https://msdn.microsoft.com/378f6f43-5c05-4ae4-be24-956f9fc0cacf">DirectShow Structures</a>



<a href="https://msdn.microsoft.com/en-us/library/Dd375997(v=VS.85).aspx">IAMVideoAccelerator::BeginFrame</a>
 

 
