---
UID: NF:memoryapi.UnmapViewOfFile
title: UnmapViewOfFile function
author: windows-sdk-content
description: Unmaps a mapped view of a file from the calling process's address space.
old-location: base\unmapviewoffile.htm
tech.root: memory
ms.assetid: 2e9c3174-af48-4fa3-9f6a-fb62b23ed994
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: UnmapViewOfFile, UnmapViewOfFile function, _win32_unmapviewoffile, base.unmapviewoffile, fs.unmapviewoffile, winbase/UnmapViewOfFile
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: memoryapi.h
req.include-header: Windows.h, Memoryapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
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
 - API-MS-Win-Core-memory-l1-1-0.dll
 - KernelBase.dll
 - API-MS-Win-Core-memory-l1-1-1.dll
 - API-MS-Win-Core-memory-l1-1-2.dll
 - API-MS-Win-Core-memory-l1-1-3.dll
 - API-MS-Win-DownLevel-Kernel32-l1-1-0.dll
 - MinKernelBase.dll
 - API-MS-Win-Core-Memory-L1-1-4.dll
api_name:
 - UnmapViewOfFile
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# UnmapViewOfFile function


## -description


Unmaps a mapped view of a file from the calling process's address space.


## -parameters




### -param lpBaseAddress [in]

A pointer to the base address of the mapped view of a file that is to be unmapped. This value must be identical to the value returned by a previous call to the 
<a href="https://msdn.microsoft.com/df9f54cd-b2de-4107-a1c5-d5a07045851e">MapViewOfFile</a> or 
<a href="https://msdn.microsoft.com/2ac8a7d6-5c52-41de-acb9-d7f975fd2a94">MapViewOfFileEx</a> function.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



Unmapping a mapped view of a file invalidates the range occupied by the view in the address space of the process and makes the range available for other allocations. It removes the working set entry for each unmapped virtual page that was part of the working set of the process and reduces the working set size of the process. It also decrements the share count of the corresponding physical page.

Modified pages in the unmapped view are not written to disk until their share count reaches zero, or in other words, until they are unmapped or trimmed from the working sets of all processes that share the pages. Even then, the modified pages are written "lazily" to disk; that is, modifications may be cached in memory and written to disk at a later time. To minimize the risk of data loss in the event of a power failure or a system crash, applications should explicitly flush modified pages using the <a href="https://msdn.microsoft.com/994fef62-77cf-4c99-be54-b4aff35a10f2">FlushViewOfFile</a> function.

Although an application may close the file handle used to create a file mapping object, the system holds the corresponding file open until the last view of the file is unmapped.  Files for which the last view has not yet been unmapped are held open with no sharing restrictions.

In Windows Server 2012, this function is supported by the following technologies.

<table>
<tr>
<th>Technology</th>
<th>Supported</th>
</tr>
<tr>
<td>
Server Message Block (SMB) 3.0 protocol

</td>
<td>
Yes

</td>
</tr>
<tr>
<td>
SMB 3.0 Transparent Failover (TFO)

</td>
<td>
Yes

</td>
</tr>
<tr>
<td>
SMB 3.0 with Scale-out File Shares (SO)

</td>
<td>
Yes

</td>
</tr>
<tr>
<td>
Cluster Shared Volume File System (CsvFS)

</td>
<td>
Yes

</td>
</tr>
<tr>
<td>
Resilient File System (ReFS)

</td>
<td>
Yes

</td>
</tr>
</table>
 


#### Examples

For an example, see 
<a href="https://msdn.microsoft.com/e47a0e79-3000-479b-afba-dcd36210ea3d">Creating a View Within a File</a>.

<div class="code"></div>



## -see-also




<a href="https://msdn.microsoft.com/d62d068c-9b1d-4dbf-8b21-31a636a41456">Closing a File Mapping Object</a>



<a href="https://msdn.microsoft.com/5a2a7a62-0bda-4a0d-93d2-25b4898871fd">File Mapping Functions</a>



<a href="https://msdn.microsoft.com/df9f54cd-b2de-4107-a1c5-d5a07045851e">MapViewOfFile</a>



<a href="https://msdn.microsoft.com/2ac8a7d6-5c52-41de-acb9-d7f975fd2a94">MapViewOfFileEx</a>



Memory
    Management Functions
 

 
