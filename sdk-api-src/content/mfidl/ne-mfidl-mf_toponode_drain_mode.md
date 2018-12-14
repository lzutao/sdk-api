---
UID: NE:mfidl._MF_TOPONODE_DRAIN_MODE
title: MF_TOPONODE_DRAIN_MODE
author: windows-sdk-content
description: Defines at what times a transform in a topology is drained.
old-location: mf\mf_toponode_drain_mode.htm
tech.root: medfound
ms.assetid: 7f84fd12-40c3-4201-8986-a2883ba2f53d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: 7f84fd12-40c3-4201-8986-a2883ba2f53d, MF_TOPONODE_DRAIN_ALWAYS, MF_TOPONODE_DRAIN_DEFAULT, MF_TOPONODE_DRAIN_MODE, MF_TOPONODE_DRAIN_MODE enumeration [Media Foundation], MF_TOPONODE_DRAIN_NEVER, mf.mf_toponode_drain_mode, mfidl/MF_TOPONODE_DRAIN_ALWAYS, mfidl/MF_TOPONODE_DRAIN_DEFAULT, mfidl/MF_TOPONODE_DRAIN_MODE, mfidl/MF_TOPONODE_DRAIN_NEVER
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - mfidl.h
api_name:
 - MF_TOPONODE_DRAIN_MODE
product: Windows
targetos: Windows
req.typenames: MF_TOPONODE_DRAIN_MODE
req.redist: 
---

# MF_TOPONODE_DRAIN_MODE enumeration


## -description



Defines at what times a transform in a topology is drained.




## -enum-fields




### -field MF_TOPONODE_DRAIN_DEFAULT

The transform is drained when the end of a stream is reached. It is not drained when markout is reached at the end of a segment.


### -field MF_TOPONODE_DRAIN_ALWAYS

The transform is drained whenever a topology ends.


### -field MF_TOPONODE_DRAIN_NEVER

The transform is never drained.


## -see-also




<a href="https://msdn.microsoft.com/68332106-d1fe-467b-8baa-1e592b9cc243">MF_TOPONODE_DRAIN</a>



<a href="https://msdn.microsoft.com/f26a730f-18c4-4247-acaf-af1dfad19086">Media Foundation Enumerations</a>
 

 
