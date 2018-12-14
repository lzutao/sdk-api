---
UID: NF:evntrace.OpenTraceA
title: OpenTraceA function
author: windows-sdk-content
description: The OpenTrace function opens a real-time trace session or log file for consuming.
old-location: etw\opentrace.htm
tech.root: etw
ms.assetid: 505e643b-6b4f-4f93-96c8-7fe8abdd6234
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: OpenTrace, OpenTrace function [ETW], OpenTraceA, OpenTraceW, _evt_opentrace, base.opentrace, etw.opentrace, evntrace/OpenTrace, evntrace/OpenTraceA, evntrace/OpenTraceW
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: evntrace.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: OpenTraceW (Unicode) and OpenTraceA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Sechost.lib on Windows 8.1 and Windows Server 2012 R2; Advapi32.lib on Windows 8, Windows Server 2012, Windows 7, Windows Server 2008 R2, Windows Server 2008, Windows Vista and Windows XP
req.dll: Sechost.dll on Windows 8.1 and Windows Server 2012 R2; Advapi32.dll on Windows 8, Windows Server 2012, Windows 7, Windows Server 2008 R2, Windows Server 2008, Windows Vista and Windows XP
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Sechost.dll
 - Advapi32.dll
 - AdvAPI32Legacy.dll
 - API-MS-Win-DownLevel-AdvAPI32-l2-1-1.dll
 - API-MS-Win-Eventing-Consumer-l1-1-0.dll
 - API-MS-Win-Eventing-Legacy-l1-1-0.dll
 - KernelBase.dll
api_name:
 - OpenTrace
 - OpenTraceA
 - OpenTraceW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# OpenTraceA function


## -description


The <b>OpenTrace</b> function opens a real-time trace session or 
   log file for consuming.


## -parameters




### -param Logfile [in, out]

Pointer to an <a href="https://msdn.microsoft.com/179451e9-7e3c-4d3a-bcc6-3ad9d382229a">EVENT_TRACE_LOGFILE</a> structure. 
      The structure specifies the source from which to consume events (from a log file or the session in real time) 
      and specifies the callbacks the consumer wants to use to receive the events. 


## -returns



If the function succeeds, it returns a handle to the trace.

If the function fails, it returns INVALID_PROCESSTRACE_HANDLE.

<div class="alert"><b>Note</b>  <p class="note">If your code base supports Windows 7 and Windows Vista, and also supports 
        earlier operating systems such as Windows XP and Windows Server 2003, do not use the 
        constants described above. Instead, determine the operating system on which you are running and compare the 
        return value to the following values.

<table>
<tr>
<th>Operating system</th>
<th>Application</th>
<th>Return value to compare</th>
</tr>
<tr>
<td>Windows 7 and Windows Vista</td>
<td>32-bit</td>
<td>0x00000000FFFFFFFF</td>
</tr>
<tr>
<td>Windows 7 and Windows Vista</td>
<td>64-bit</td>
<td>0XFFFFFFFFFFFFFFFF</td>
</tr>
<tr>
<td>Windows XP and Windows Server 2003</td>
<td>32- or 64-bit</td>
<td>0XFFFFFFFFFFFFFFFF</td>
</tr>
</table>
 

</div>
<div> </div>
If the function returns INVALID_PROCESSTRACE_HANDLE, you can use the 
       <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> function to obtain extended error 
       information. The following table lists some common errors and their causes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The <i>Logfile</i> parameter is <b>NULL</b>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_BAD_PATHNAME</b></dt>
</dl>
</td>
<td width="60%">
If you did not specify the <b>LoggerName</b> member of <a href="https://msdn.microsoft.com/179451e9-7e3c-4d3a-bcc6-3ad9d382229a">EVENT_TRACE_LOGFILE</a>, you must specify a valid log file name.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
Only users with administrative privileges, users in the Performance Log Users group, and services running 
         as LocalSystem, LocalService, NetworkService can consume events in real time. To grant a restricted user the 
         ability to consume events in real time, add them to the Performance Log Users group.

<b>Windows XP and Windows 2000:  </b>Anyone can consume real time events.

</td>
</tr>
</table>
 




## -remarks



Consumers call this function.

After calling <b>OpenTrace</b>, call the 
    <a href="https://msdn.microsoft.com/aea25a95-f435-4068-9b15-7473f31ebf16">ProcessTrace</a> function to process the events. When you have 
    finished processing events, call the <a href="https://msdn.microsoft.com/25f4c4d3-0b70-40fe-bf03-8f9ffd82fbec">CloseTrace</a> 
    function.

Note that you can process events from only one real-time session.

Windows Vista and earlier: If the function fails it will returns INVALID_HANDLE_VALUE. To avoid 
    compile-time errors, cast INVALID_HANDLE_VALUE to TRACEHANDLE as follows: 
    <code>(TRACEHANDLE)INVALID_HANDLE_VALUE</code>.


#### Examples

For an example that uses <b>OpenTrace</b>, see 
     <a href="https://msdn.microsoft.com/5ebd500c-420e-4979-a03a-49b687464b0e">Using TdhFormatProperty to Consume Event Data</a> 
     or <a href="https://msdn.microsoft.com/13512236-c416-43ba-bf36-b05c5c08d6c9">Retrieving Event Data Using MOF</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/25f4c4d3-0b70-40fe-bf03-8f9ffd82fbec">CloseTrace</a>



<a href="https://msdn.microsoft.com/179451e9-7e3c-4d3a-bcc6-3ad9d382229a">EVENT_TRACE_LOGFILE</a>



<a href="https://msdn.microsoft.com/aea25a95-f435-4068-9b15-7473f31ebf16">ProcessTrace</a>
 

 
