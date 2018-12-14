---
UID: NC:filehc.FCACHE_RICHCREATE_CALLBACK
title: FCACHE_RICHCREATE_CALLBACK
author: windows-sdk-content
description: A callback function that is used to create items in the cache.
old-location: winprog\fcache_richcreate_callback.htm
tech.root: devnotes
ms.assetid: 86e0d47e-469b-4c1d-9e39-f4f6d9e58ba0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FCACHE_RICHCREATE_CALLBACK, FCACHE_RICHCREATE_CALLBACK callback, FCACHE_RICHCREATE_CALLBACK callback function [Windows API], filehc/FCACHE_RICHCREATE_CALLBACK, winprog.fcache_richcreate_callback
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
 - FCACHE_RICHCREATE_CALLBACK
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# FCACHE_RICHCREATE_CALLBACK callback function


## -description


A callback function that is used to create items in the cache. It is called by <a href="https://msdn.microsoft.com/89b0adcd-0084-4538-b162-661ddae53dc8">CacheRichCreateFile</a>.


## -parameters




### -param lpstrName [in]

The name of the file.


### -param lpvData [in]

User-provided data to <a href="https://msdn.microsoft.com/89b0adcd-0084-4538-b162-661ddae53dc8">CacheRichCreateFile</a>.


### -param *cbFileSize [out]

The size of the low <b>DWORD</b>.


### -param *cbFileSizeHigh [out]

The size of the high <b>DWORD</b>.


### -param *pfDidWeScanIt [out]

Set to <b>TRUE</b> if the file has been scanned; otherwise, it is set to <b>FALSE</b>.


### -param *pfIsStuffed [out]

Set to <b>TRUE</b> if the file is dot stuffed; otherwise, it is set to <b>FALSE</b>.


### -param *pfStoredWithDots [out]

If set to <b>TRUE</b>, this parameter indicates that any dots  that appear at the beginning of a line are stored with an extra dot as required in NNTP, SMTP, and POP3 protocols. If this is <b>FALSE</b>, the message is stored without dot stuffing.


### -param *pfStoredWithTerminatingDot [out]

If set to <b>TRUE</b>, the file has been stored with a terminating dot; otherwise, it is <b>FALSE</b>.


## -returns



Returns a handle to the file that was created in the cache.




## -see-also




<a href="https://msdn.microsoft.com/89b0adcd-0084-4538-b162-661ddae53dc8">CacheRichCreateFile</a>
 

 
