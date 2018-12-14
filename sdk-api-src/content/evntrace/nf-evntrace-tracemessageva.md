---
UID: NF:evntrace.TraceMessageVa
title: TraceMessageVa function
author: windows-sdk-content
description: The TraceMessageVa function sends an informational message with variable arguments to an event tracing session.
old-location: etw\tracemessageva.htm
tech.root: etw
ms.assetid: 2cfb7226-fd29-432e-abfd-bd10c6344a67
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PVOID, TRACE_MESSAGE_GUID, TRACE_MESSAGE_SEQUENCE, TRACE_MESSAGE_SYSTEMINFO, TRACE_MESSAGE_TIMESTAMP, TraceMessageVa, TraceMessageVa function [ETW], _evt_tracemessageva, base.tracemessageva, etw.tracemessageva, evntrace/TraceMessageVa, size_t
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: evntrace.h
req.include-header: 
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
req.lib: Advapi32.lib
req.dll: Advapi32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Advapi32.dll
 - API-MS-Win-DownLevel-AdvApi32-l1-1-0.dll
 - KernelBase.dll
 - API-MS-Win-DownLevel-AdvApi32-l1-1-1.dll
 - API-MS-Win-eventing-classicprovider-l1-1-0.dll
api_name:
 - TraceMessageVa
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TraceMessageVa function


## -description


The 
<b>TraceMessageVa</b> function sends an informational message with variable arguments to an event tracing session. 


## -parameters




### -param LoggerHandle [in]

Handle to the event tracing session that records the event. The provider obtains the handle when it calls the <a href="https://msdn.microsoft.com/050d3a01-0087-40f1-af35-b9ceeaf47813">GetTraceLoggerHandle</a> function in its <a href="https://msdn.microsoft.com/e9f70ae6-906f-4e55-bca7-4355f1ca6091">ControlCallback</a> implementation.


### -param MessageFlags [in]

Adds additional information to the beginning of the provider-specific data section of the event. The provider-specific data section of the event will contain data only for those flags that are set. The variable list of argument data will follow this information. This parameter can be one or more of the following values. 



<table>
<tr>
<th>Flag</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="TRACE_MESSAGE_GUID"></a><a id="trace_message_guid"></a><dl>
<dt><b>TRACE_MESSAGE_GUID</b></dt>
</dl>
</td>
<td width="60%">
Include the event trace class GUID in the message. The <i>MessageGuid</i> parameter contains the event trace class  GUID.

</td>
</tr>
<tr>
<td width="40%"><a id="TRACE_MESSAGE_SEQUENCE"></a><a id="trace_message_sequence"></a><dl>
<dt><b>TRACE_MESSAGE_SEQUENCE</b></dt>
</dl>
</td>
<td width="60%">
Include a sequence number in the message. The sequence number starts at one. To use this flag, the controller must have set the <b>EVENT_TRACE_USE_GLOBAL_SEQUENCE</b> or <b>EVENT_TRACE_USE_LOCAL_SEQUENCE</b> log file mode when creating the session.

</td>
</tr>
<tr>
<td width="40%"><a id="TRACE_MESSAGE_SYSTEMINFO"></a><a id="trace_message_systeminfo"></a><dl>
<dt><b>TRACE_MESSAGE_SYSTEMINFO</b></dt>
</dl>
</td>
<td width="60%">
Include the thread identifier and process identifier in the message.

</td>
</tr>
<tr>
<td width="40%"><a id="TRACE_MESSAGE_TIMESTAMP"></a><a id="trace_message_timestamp"></a><dl>
<dt><b>TRACE_MESSAGE_TIMESTAMP</b></dt>
</dl>
</td>
<td width="60%">
Include a time stamp in the message.

</td>
</tr>
</table>
 

The information is included in the event data in the following order:

<ul>
<li>Sequence number</li>
<li>Event trace class GUID</li>
<li>Time stamp</li>
<li>Thread identifier</li>
<li>Process identifier</li>
</ul>

### -param MessageGuid [in]

Class GUID that identifies the event trace message.


### -param MessageNumber [in]

Number that uniquely identifies each occurrence of the message. You must define the value specified for this parameter; the value should be meaningful to the application.


### -param MessageArgList [in]

List of variable arguments to be appended to the message. The list must be composed of pairs of arguments, as described in the following table. 



<table>
<tr>
<th>Data Type</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="PVOID"></a><a id="pvoid"></a><dl>
<dt><b>PVOID</b></dt>
</dl>
</td>
<td width="60%">
Pointer to the argument data.

</td>
</tr>
<tr>
<td width="40%"><a id="size_t"></a><a id="SIZE_T"></a><dl>
<dt><b>size_t</b></dt>
</dl>
</td>
<td width="60%">
The size of the argument data, in bytes.

</td>
</tr>
</table>
 

Terminate the list using an argument pair consisting of a pointer to <b>NULL</b> and zero.
						
						

The caller must ensure that the sum of the sizes of the arguments + 72 does not exceed the size of the event tracing session's buffer.


## -returns



If the function succeeds, the return value is ERROR_SUCCESS.
						

If the function fails, the return value is one of the 
<a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error codes</a>. The following table includes some common errors and their causes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_HANDLE</b></dt>
</dl>
</td>
<td width="60%">
Either the <i>SessionHandle</i> is <b>NULL</b> or specifies the NT Kernel Logger session handle.
							

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
The session ran out of free buffers to write to. This can occur during high event rates because the disk subsystem is overloaded or the number of buffers is too small. Rather than blocking until more buffers become available, <a href="https://msdn.microsoft.com/5d81c851-d47e-43f8-97b0-87156f36119a">TraceMessage</a> discards the event.

<b>Windows 2000 and Windows XP:  </b>Not supported.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
The event is discarded because, although the buffer pool has not reached its maximum size, there is insufficient available memory to allocate an additional buffer and there is no buffer available to receive the event. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
<i>MessageFlags</i> contains a value that is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_MORE_DATA</b></dt>
</dl>
</td>
<td width="60%">
Data from a single event cannot span multiple buffers. A trace event is limited to the size of the event tracing session's buffer minus the size of the  
<a href="https://msdn.microsoft.com/33c2de6b-afc2-4323-8d81-2970e66edf5e">EVENT_TRACE_HEADER</a> structure. 

</td>
</tr>
</table>
 




## -remarks



Providers call this function.

Using the <a href="https://msdn.microsoft.com/9b21f6f0-dd9b-4f9c-a879-846901a3bab7">TraceEvent</a> function is the preferred way to log an event. On Windows Vista, you should use the <a href="https://msdn.microsoft.com/93070eb7-c167-4419-abff-e861877dad07">EventWrite</a> function to log events.

The trace events are written in the order in which they occur. 

If you do not need to access the message tracing functionality from a wrapper function, you can call the 
<a href="https://msdn.microsoft.com/5d81c851-d47e-43f8-97b0-87156f36119a">TraceMessage</a> version of this function.

Consumers will have to use the <a href="https://msdn.microsoft.com/9312eaed-2997-4d44-952a-fcae3b262947">EventCallback</a> callback to receive and process the events if the <i>MessageFlags</i> parameter does not contain the TRACE_MESSAGE_GUID flag. If you do not specify the TRACE_MESSAGE_GUID flag, the consumer will not be able to use the <a href="https://msdn.microsoft.com/32e94f58-b8b6-4e0a-b53b-716a534ac374">EventClassCallback</a> because the <b>Header.Guid</b> member of the   <a href="https://msdn.microsoft.com/d8a6b63e-0cd4-4d19-b0b3-16bb0d33e4c0">EVENT_TRACE</a> structure will not contain the event trace class GUID.

Note that the members of the <a href="https://msdn.microsoft.com/d8a6b63e-0cd4-4d19-b0b3-16bb0d33e4c0">EVENT_TRACE</a> and <a href="https://msdn.microsoft.com/33c2de6b-afc2-4323-8d81-2970e66edf5e">EVENT_TRACE_HEADER</a> structures that correspond to the <i>MessageFlags</i> flags are set only if the corresponding flag is specified. For example, the <b>ThreadId</b> and <b>ProcessId</b> members of <b>EVENT_TRACE_HEADER</b> are populated only if you specify the TRACE_MESSAGE_SYSTEMINFO flag.




## -see-also




<a href="https://msdn.microsoft.com/9b21f6f0-dd9b-4f9c-a879-846901a3bab7">TraceEvent</a>



<a href="https://msdn.microsoft.com/e8361bdc-21dd-47a0-bdbf-56f4d6195689">TraceEventInstance</a>



<a href="https://msdn.microsoft.com/5d81c851-d47e-43f8-97b0-87156f36119a">TraceMessage</a>
 

 
