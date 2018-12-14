---
UID: NC:filehc.CACHE_READ_CALLBACK
title: CACHE_READ_CALLBACK
author: windows-sdk-content
description: A callback that is provided to the cache to help examine items within the cache.
old-location: winprog\fcache_read_callback.htm
tech.root: devnotes
ms.assetid: 9fcdbca6-95db-4ec1-b81c-3681e9e2bffb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CACHE_READ_CALLBACK, CACHE_READ_CALLBACK callback, CACHE_READ_CALLBACK callback function [Windows API], filehc/CACHE_READ_CALLBACK, winprog.fcache_read_callback
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: filehc.h
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
 - UserDefined
api_location:
 - Filehc.h
api_name:
 - CACHE_READ_CALLBACK
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CACHE_READ_CALLBACK callback function


## -description


A callback that is provided to the cache to help examine items within the cache.


## -parameters




### -param cb [in]

The size, in bytes, of the data indicated in the <i>lpb</i> parameter.


### -param lpb [in]

A pointer to the data portion of the key.


### -param lpvContext [in]

The context that is specified by the user.


## -returns



Returns <b>TRUE</b> if the function succeeds; otherwise, it returns <b>FALSE</b>.

<div class="alert"><b>Note</b>  This return value is ignored.</div>
<div> </div>

