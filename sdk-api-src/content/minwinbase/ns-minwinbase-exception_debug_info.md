---
UID: NS:minwinbase._EXCEPTION_DEBUG_INFO
title: EXCEPTION_DEBUG_INFO
author: windows-sdk-content
description: Contains exception information that can be used by a debugger.
old-location: base\exception_debug_info_str.htm
tech.root: debug
ms.assetid: f5917ae3-cc45-42c4-a3fb-5d0aef2a3bdb
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPEXCEPTION_DEBUG_INFO, EXCEPTION_DEBUG_INFO, EXCEPTION_DEBUG_INFO structure, LPEXCEPTION_DEBUG_INFO, LPEXCEPTION_DEBUG_INFO structure pointer, _EXCEPTION_DEBUG_INFO, _win32_exception_debug_info_str, base.exception_debug_info_str, minwinbase/EXCEPTION_DEBUG_INFO, minwinbase/LPEXCEPTION_DEBUG_INFO"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: minwinbase.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
 - minwinbase.h
api_name:
 - EXCEPTION_DEBUG_INFO
product: Windows
targetos: Windows
req.typenames: EXCEPTION_DEBUG_INFO, *LPEXCEPTION_DEBUG_INFO
req.redist: 
---

# EXCEPTION_DEBUG_INFO structure


## -description


Contains exception information that can be used by a debugger.


## -struct-fields




### -field ExceptionRecord

An 
<a href="https://msdn.microsoft.com/85a64178-bdcb-4293-9363-289c654730a2">EXCEPTION_RECORD</a> structure with information specific to the exception. This includes the exception code, flags, address, a pointer to a related exception, extra parameters, and so on.


### -field dwFirstChance

A value that indicates whether the debugger has previously encountered the exception specified by the <b>ExceptionRecord</b> member. If the <b>dwFirstChance</b> member is nonzero, this is the first time the debugger has encountered the exception. Debuggers typically handle breakpoint and single-step exceptions when they are first encountered. If this member is zero, the debugger has previously encountered the exception. This occurs only if, during the search for structured exception handlers, either no handler was found or the exception was continued.


## -see-also




<a href="https://msdn.microsoft.com/056aa7ee-51ca-48ec-9cd7-26085bb85b11">DEBUG_EVENT</a>



<a href="https://msdn.microsoft.com/85a64178-bdcb-4293-9363-289c654730a2">EXCEPTION_RECORD</a>
 

 
