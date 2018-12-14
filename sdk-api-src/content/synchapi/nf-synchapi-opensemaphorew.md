---
UID: NF:synchapi.OpenSemaphoreW
title: OpenSemaphoreW function
author: windows-sdk-content
description: Opens an existing named semaphore object.
old-location: base\opensemaphore.htm
tech.root: sync
ms.assetid: 2ea525b9-f33d-4b72-85e1-6d2cfdc64f5f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: OpenSemaphore, OpenSemaphore function, OpenSemaphoreA, OpenSemaphoreW, _win32_opensemaphore, base.opensemaphore, synchapi/OpenSemaphore, synchapi/OpenSemaphoreA, synchapi/OpenSemaphoreW
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: synchapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: OpenSemaphoreW (Unicode) and OpenSemaphoreA (ANSI)
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
 - API-MS-Win-Core-Synch-l1-1-0.dll
 - KernelBase.dll
 - API-MS-Win-Core-Synch-l1-2-0.dll
 - API-MS-Win-Core-Synch-l1-2-1.dll
 - API-MS-Win-DownLevel-Kernel32-l1-1-0.dll
 - MinKernelBase.dll
 - API-MS-Win-Core-Synch-Ansi-L1-1-0.dll
 - Kernel32Legacy.dll
api_name:
 - OpenSemaphore
 - OpenSemaphoreA
 - OpenSemaphoreW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# OpenSemaphoreW function


## -description


Opens an existing named semaphore object.


## -parameters




### -param dwDesiredAccess [in]

The access to the semaphore object. The function fails if the security descriptor of the specified object does not permit the requested access for the calling process. For a list of access rights, see 
<a href="https://msdn.microsoft.com/92478298-617c-4672-a1cc-9a8e9af40327">Synchronization Object Security and Access Rights</a>. 





### -param bInheritHandle [in]

If this value is <b>TRUE</b>, processes created by this process will inherit the handle. Otherwise, the processes do not inherit this handle.


### -param lpName [in]

The name of the semaphore to be opened. Name comparisons are case sensitive. 




This function can open objects in a private namespace. For more information, see <a href="https://msdn.microsoft.com/6a84ec16-fa65-4cdd-861a-eccf5d0eee2b">Object Namespaces</a>.

<b>Terminal Services:  </b>The name can have a "Global\" or "Local\" prefix to explicitly open an object in the global or session namespace. The remainder of the name can contain any character except the backslash character (\). For more information, see 
<a href="https://msdn.microsoft.com/771e0bbf-bd73-4e87-aa1e-945c1287b517">Kernel Object Namespaces</a>.

<b>Note</b>  Fast user switching is implemented using Terminal Services sessions. The first user to log on uses session 0, the next user to log on uses session 1, and so on. Kernel object names must follow the guidelines outlined for Terminal Services so that applications can support multiple users.


## -returns



If the function succeeds, the return value is a handle to the semaphore object.

If the function fails, the return value is <b>NULL</b>. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The 
<b>OpenSemaphore</b> function enables multiple processes to open handles of the same semaphore object. The function succeeds only if some process has already created the semaphore by using the 
<a href="https://msdn.microsoft.com/2e55d67b-99de-4f10-8637-00d9d62e4460">CreateSemaphore</a> function. The calling process can use the returned handle in any function that requires a handle to a semaphore object, such as the 
<a href="https://msdn.microsoft.com/9c66c71d-fdfd-42ae-895c-2fc842b5bc7a">wait functions</a>, subject to the limitations of the access specified in the <i>dwDesiredAccess</i> parameter.

The handle can be duplicated by using the <a href="https://msdn.microsoft.com/9c8da574-5bda-49f1-a6b6-c026639d6504">DuplicateHandle</a> function. Use the <a href="https://msdn.microsoft.com/9b84891d-62ca-4ddc-97b7-c4c79482abd9">CloseHandle</a> function to close the handle. The system closes the handle automatically when the process terminates. The semaphore object is destroyed when its last handle has been closed.




## -see-also




<a href="https://msdn.microsoft.com/9b84891d-62ca-4ddc-97b7-c4c79482abd9">CloseHandle</a>



<a href="https://msdn.microsoft.com/2e55d67b-99de-4f10-8637-00d9d62e4460">CreateSemaphore</a>



<a href="https://msdn.microsoft.com/9c8da574-5bda-49f1-a6b6-c026639d6504">DuplicateHandle</a>



<a href="https://msdn.microsoft.com/00a00227-45fc-49a1-8ff5-aeccb172d16a">Object Names</a>



<a href="https://msdn.microsoft.com/9d444318-4d66-4ec3-a65d-bd3b75db9d9b">ReleaseSemaphore</a>



<a href="https://msdn.microsoft.com/d9da1d98-a306-4e2d-a149-1eef6a724751">Semaphore Objects</a>



<a href="https://msdn.microsoft.com/9b6359c2-0113-49b6-83d0-316ad95aba1b">Synchronization Functions</a>
 

 
