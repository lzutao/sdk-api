---
UID: NF:memoryapi.WriteProcessMemory
title: WriteProcessMemory function
author: windows-sdk-content
description: Writes data to an area of memory in a specified process. The entire area to be written to must be accessible or the operation fails.
old-location: base\writeprocessmemory.htm
tech.root: debug
ms.assetid: 9cd91f1c-58ce-4adc-b027-45748543eb06
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WriteProcessMemory, WriteProcessMemory function, _win32_writeprocessmemory, base.writeprocessmemory, memoryapi/WriteProcessMemory
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: memoryapi.h
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
 - WriteProcessMemory
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WriteProcessMemory function


## -description


Writes data to an area of memory in a specified process. The entire area to be written to must be accessible or the operation fails.


## -parameters




### -param hProcess [in]

A handle to the process memory to be modified. The handle must have PROCESS_VM_WRITE and PROCESS_VM_OPERATION access to the process.


### -param lpBaseAddress [in]

A pointer to the base address in the specified process to which data is written. Before data transfer occurs, the system verifies that all data in the base address and memory of the specified size is accessible for write access, and if it is not accessible, the function fails.


### -param lpBuffer [in]

A pointer to the buffer that contains data to be written in  the address space of the specified process.


### -param nSize [in]

The number of bytes to be written to the specified process.


### -param lpNumberOfBytesWritten [out]

A pointer to a variable that receives the number of bytes transferred into the specified process. This parameter is optional. If <i>lpNumberOfBytesWritten</i> is <b>NULL</b>, the parameter is ignored.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is 0 (zero). To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. The function fails if the requested write operation crosses into an area of the process that is inaccessible.




## -remarks



<b>WriteProcessMemory</b> copies the data from the specified buffer in the current process to the address range of the specified process. Any process that has a handle with PROCESS_VM_WRITE and PROCESS_VM_OPERATION access to the process to be written to can call the function. Typically but not always, the process with address space that is being written to is  being debugged.

The entire area to be written to must be accessible, and if it is not accessible, the function fails.




## -see-also




<a href="https://msdn.microsoft.com/95a838a2-f138-4682-b733-3f363b6c4a4b">Debugging Functions</a>



<a href="https://msdn.microsoft.com/7056e181-9bc5-4530-a7b8-d5ff1e345eef">Process Functions for Debugging</a>



<a href="https://msdn.microsoft.com/8774e145-ee7f-44de-85db-0445b905f986">ReadProcessMemory</a>



<a href="https://msdn.microsoft.com/ff0b6b79-40f5-499c-b797-b66797654164">VirtualAllocEx</a>
 

 
