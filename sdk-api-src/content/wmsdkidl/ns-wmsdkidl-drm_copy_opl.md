---
UID: NS:wmsdkidl.__tagDRM_COPY_OPL
title: DRM_COPY_OPL
author: windows-sdk-content
description: The DRM_COPY_OPL structure holds information about the output protection levels specified in a license for copy actions.
old-location: wmformat\drm_copy_opl.htm
tech.root: wmformat
ms.assetid: cf35626a-5583-440f-8f17-0c9b79bd843d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DRM_COPY_OPL, DRM_COPY_OPL structure [windows Media Format], structure [windows Media Format], wmformat.drm_copy_opl, wmsdkidl/DRM_COPY_OPL
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: wmsdkidl.h
req.include-header: Drmexternals.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only],Windows Media Format 9.5 SDK
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - wmsdkidl.h
api_name:
 - DRM_COPY_OPL
product: Windows
targetos: Windows
req.typenames: DRM_COPY_OPL
req.redist: 
---

# DRM_COPY_OPL structure


## -description



The <b>DRM_COPY_OPL</b> structure holds information about the output protection levels specified in a license for copy actions.




## -struct-fields




### -field wMinimumCopyLevel

Minimum output protection level for copy actions.


### -field oplIdIncludes


<a href="https://msdn.microsoft.com/a1f0e1ad-0ba4-4c42-aff5-c5fb4133e0fa">DRM_OPL_OUTPUT_IDS</a> structure containing the identifiers of technologies to allow. This member is used for output technologies that are assigned OPLs lower than the minimum copy level, but to which the content may be copied.


### -field oplIdExcludes


<a href="https://msdn.microsoft.com/a1f0e1ad-0ba4-4c42-aff5-c5fb4133e0fa">DRM_OPL_OUTPUT_IDS</a> structure containing the output identifiers of technologies to restrict. This member is used for output technologies that are assigned OPLs that exceed the minimum copy level, but that the license issuer does not grant rights for copying to.


## -see-also




<a href="https://msdn.microsoft.com/5d14bd02-0fb5-4982-b3dc-7f8277cb852f">DRM_PLAY_OPL</a>



<a href="https://msdn.microsoft.com/118ef278-ca4f-4c30-9633-a2d851f5c758">Structures</a>
 

 
