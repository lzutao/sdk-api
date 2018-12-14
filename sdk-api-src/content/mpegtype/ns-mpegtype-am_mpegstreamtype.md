---
UID: NS:mpegtype.tagAM_MPEGSTREAMTYPE
title: AM_MPEGSTREAMTYPE
author: windows-sdk-content
description: The AM_MPEGSTREAMTYPE structure defines the media type for an MPEG-1 program stream.
old-location: dshow\am_mpegstreamtype.htm
tech.root: DirectShow
ms.assetid: 8622ffcb-be64-4a8f-8bc7-834b559b0f95
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AM_MPEGSTREAMTYPE, AM_MPEGSTREAMTYPE structure [DirectShow], dshow.am_mpegstreamtype, mpegtype/AM_MPEGSTREAMTYPE
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: mpegtype.h
req.include-header: Dshow.h
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
 - mpegtype.h
api_name:
 - AM_MPEGSTREAMTYPE
product: Windows
targetos: Windows
req.typenames: AM_MPEGSTREAMTYPE
req.redist: 
---

# AM_MPEGSTREAMTYPE structure


## -description


The <b>AM_MPEGSTREAMTYPE</b> structure defines the media type for an MPEG-1 program stream.
        


## -struct-fields




### -field dwStreamId

 


### -field dwReserved

Reserved.


### -field mt


<a href="https://msdn.microsoft.com/en-us/library/Dd373477(v=VS.85).aspx">AM_MEDIA_TYPE</a> structure describing the type for the substeam. The <b>pbFormat</b> member of this structure must <b>NULL</b>. The format data normally conveyed in <b>pbFormat</b> is stored in the <b>bFormat</b> member.


### -field bFormat

Format data. The size of this array, in bytes, is given in the <b>mt.cbFormat</b> member.


#### - dwStreamID

Stream identifier of the stream to process.


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd373481(v=VS.85).aspx">AM_MPEGSYSTEMTYPE</a>



<a href="https://msdn.microsoft.com/378f6f43-5c05-4ae4-be24-956f9fc0cacf">DirectShow Structures</a>



<a href="https://msdn.microsoft.com/4ea1cb84-0558-4c4a-9483-1b0f2a8f76f8">MEPG-1 Media Types</a>
 

 
