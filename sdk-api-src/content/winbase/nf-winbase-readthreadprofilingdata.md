---
UID: NF:winbase.ReadThreadProfilingData
title: ReadThreadProfilingData function
author: windows-sdk-content
description: Reads the specified profiling data associated with the thread.
old-location: hcp\readthreadprofilingdata.htm
tech.root: hcp
ms.assetid: e7335caf-d89b-45b4-831d-9ead4448a6a3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: READ_THREAD_PROFILING_FLAG_DISPATCHING, READ_THREAD_PROFILING_FLAG_HARDWARE_COUNTERS, ReadThreadProfilingData, ReadThreadProfilingData function [Hardware Counter Profiling], hcp.readthreadprofilingdata, winbase/ReadThreadProfilingData
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winbase.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
api_name:
 - ReadThreadProfilingData
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ReadThreadProfilingData function


## -description


Reads the specified profiling data associated with the thread.


## -parameters




### -param PerformanceDataHandle [in]

The handle that the <a href="https://msdn.microsoft.com/dbbe5b01-cabf-42cb-9ed9-c2c143f9923b">EnableThreadProfiling</a> function returned.


### -param Flags [in]

One or more of the following flags that specify the counter data to read. The flags must have been set when you called the <a href="https://msdn.microsoft.com/dbbe5b01-cabf-42cb-9ed9-c2c143f9923b">EnableThreadProfiling</a> function.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="READ_THREAD_PROFILING_FLAG_DISPATCHING"></a><a id="read_thread_profiling_flag_dispatching"></a><dl>
<dt><b>READ_THREAD_PROFILING_FLAG_DISPATCHING</b></dt>
<dt>0x00000001</dt>
</dl>
</td>
<td width="60%">
Get the thread profiling data.

</td>
</tr>
<tr>
<td width="40%"><a id="READ_THREAD_PROFILING_FLAG_HARDWARE_COUNTERS"></a><a id="read_thread_profiling_flag_hardware_counters"></a><dl>
<dt><b>READ_THREAD_PROFILING_FLAG_HARDWARE_COUNTERS</b></dt>
<dt>0x00000002</dt>
</dl>
</td>
<td width="60%">
Get the hardware performance counters data.

</td>
</tr>
</table>
 


### -param PerformanceData [out]

A <a href="https://msdn.microsoft.com/468060cc-7b17-4ef4-8ae0-74d2bfcd5e4a">PERFORMANCE_DATA</a> structure that contains the thread profiling and hardware counter data.


## -returns



 Returns ERROR_SUCCESS if the call is successful; otherwise, a system error code (see Winerror.h).




## -see-also




<a href="https://msdn.microsoft.com/dbbe5b01-cabf-42cb-9ed9-c2c143f9923b">EnableThreadProfiling</a>
 

 
