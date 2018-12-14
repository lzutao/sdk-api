---
UID: NE:bits.__MIDL_IBackgroundCopyError_0001
title: BG_ERROR_CONTEXT
author: windows-sdk-content
description: The BG_ERROR_CONTEXT enumeration defines the constant values that specify the context in which the error occurred.
old-location: bits\bg_error_context.htm
tech.root: bits
ms.assetid: c9d98518-6f2e-4fd1-b0ee-6735c6d6ecd9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BG_ERROR_CONTEXT, BG_ERROR_CONTEXT enumeration [BITS], BG_ERROR_CONTEXT_GENERAL_QUEUE_MANAGER, BG_ERROR_CONTEXT_GENERAL_TRANSPORT, BG_ERROR_CONTEXT_LOCAL_FILE, BG_ERROR_CONTEXT_NONE, BG_ERROR_CONTEXT_QUEUE_MANAGER_NOTIFICATION, BG_ERROR_CONTEXT_REMOTE_APPLICATION, BG_ERROR_CONTEXT_REMOTE_FILE, BG_ERROR_CONTEXT_UNKNOWN, _drz_bg_error_context, bits.bg_error_context, bits/BG_ERROR_CONTEXT, bits/BG_ERROR_CONTEXT_GENERAL_QUEUE_MANAGER, bits/BG_ERROR_CONTEXT_GENERAL_TRANSPORT, bits/BG_ERROR_CONTEXT_LOCAL_FILE, bits/BG_ERROR_CONTEXT_NONE, bits/BG_ERROR_CONTEXT_QUEUE_MANAGER_NOTIFICATION, bits/BG_ERROR_CONTEXT_REMOTE_APPLICATION, bits/BG_ERROR_CONTEXT_REMOTE_FILE, bits/BG_ERROR_CONTEXT_UNKNOWN
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: bits.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP
req.target-min-winversvr: Windows Server 2003
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
 - Bits.h
api_name:
 - BG_ERROR_CONTEXT
product: Windows
targetos: Windows
req.typenames: BG_ERROR_CONTEXT
req.redist: 
---

# BG_ERROR_CONTEXT enumeration


## -description


The 
<b>BG_ERROR_CONTEXT</b> enumeration defines the constant values that specify the context in which the error occurred.


## -enum-fields




### -field BG_ERROR_CONTEXT_NONE

An error has not occurred.


### -field BG_ERROR_CONTEXT_UNKNOWN

The error context is unknown.


### -field BG_ERROR_CONTEXT_GENERAL_QUEUE_MANAGER

The transfer queue manager generated the error.


### -field BG_ERROR_CONTEXT_QUEUE_MANAGER_NOTIFICATION

The error was generated while the queue manager was notifying the client of an event.


### -field BG_ERROR_CONTEXT_LOCAL_FILE

The error was related to the specified local file. For example, permission was denied or the volume was unavailable.


### -field BG_ERROR_CONTEXT_REMOTE_FILE

The error was related to the specified remote file. For example, the URL was not accessible.


### -field BG_ERROR_CONTEXT_GENERAL_TRANSPORT

The transport layer generated the error. These errors are general transport failures  (these errors  are not specific to the remote file).


### -field BG_ERROR_CONTEXT_REMOTE_APPLICATION

The server application that BITS passed the upload file to generated an error while processing the upload file. 

<b>BITS 1.2 and earlier:  </b>Not supported.


## -see-also




<a href="https://msdn.microsoft.com/abdf115d-3ff2-4664-b053-f55872ad24ab">IBackgroundCopyError::GetError</a>



<a href="https://msdn.microsoft.com/87f5ae62-c171-4637-bebb-3a5c5aa546b3">IBackgroundCopyError::GetErrorContextDescription</a>
 

 
