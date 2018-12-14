---
UID: NS:compressapi._COMPRESS_ALLOCATION_ROUTINES
title: COMPRESS_ALLOCATION_ROUTINES
author: windows-sdk-content
description: A structure containing optional memory allocation and deallocation routines.
old-location: cmpapi\compress_allocation_routines.htm
tech.root: cmpapi
ms.assetid: 91f541c8-36b9-4ec2-ae37-0b41aa6fd623
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCOMPRESS_ALLOCATION_ROUTINES, COMPRESS_ALLOCATION_ROUTINES, COMPRESS_ALLOCATION_ROUTINES structure [Compression API], PCOMPRESS_ALLOCATION_ROUTINES, PCOMPRESS_ALLOCATION_ROUTINES structure pointer [Compression API], cmpapi.compress_allocation_routines, compressapi/COMPRESS_ALLOCATION_ROUTINES, compressapi/PCOMPRESS_ALLOCATION_ROUTINES"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: compressapi.h
req.include-header: 
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
 - compressapi.h
api_name:
 - COMPRESS_ALLOCATION_ROUTINES
product: Windows
targetos: Windows
req.typenames: COMPRESS_ALLOCATION_ROUTINES, *PCOMPRESS_ALLOCATION_ROUTINES
req.redist: 
---

# COMPRESS_ALLOCATION_ROUTINES structure


## -description


A structure containing optional memory allocation and deallocation routines.


## -struct-fields




### -field Allocate

Callback that allocates memory.


### -field Free

Callback that deallocates memory.


### -field UserContext

A pointer to context information for the allocation or deallocation routine defined by the user.
