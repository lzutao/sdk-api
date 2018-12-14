---
UID: NF:sysinfoapi.GetLogicalProcessorInformation
title: GetLogicalProcessorInformation function
author: windows-sdk-content
description: Retrieves information about logical processors and related hardware.
old-location: base\getlogicalprocessorinformation.htm
tech.root: procthread
ms.assetid: 904d2d35-f419-4e8f-a689-f39ed926644c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLogicalProcessorInformation, GetLogicalProcessorInformation function, base.getlogicalprocessorinformation, sysinfoapi/GetLogicalProcessorInformation
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: sysinfoapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP Professional x64 Edition, Windows XP with SP3 [desktop apps \| UWP apps]
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
 - API-MS-Win-Core-SysInfo-l1-1-0.dll
 - KernelBase.dll
 - API-MS-Win-Core-SysInfo-l1-2-0.dll
 - API-MS-Win-Core-SysInfo-l1-2-1.dll
 - API-MS-Win-Core-SysInfo-l1-2-2.dll
 - API-MS-Win-DownLevel-Kernel32-l1-1-0.dll
 - MinKernelBase.dll
 - API-MS-Win-Core-SysInfo-l1-2-3.dll
api_name:
 - GetLogicalProcessorInformation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetLogicalProcessorInformation function


## -description



Retrieves information about logical processors and related hardware.



To retrieve information about logical processors and related hardware, including processor groups, use the <a href="https://msdn.microsoft.com/dfc4f444-4651-4a02-b8f6-f30d9278eae2">GetLogicalProcessorInformationEx</a> function.


## -parameters




### -param Buffer [out]

A pointer to a buffer that receives  an array of <a href="https://msdn.microsoft.com/32ef5dd8-c00d-44ee-a291-a18653beb1b9">SYSTEM_LOGICAL_PROCESSOR_INFORMATION</a> structures. If the function fails, the contents of this buffer are undefined.


### -param ReturnedLength [in, out]

On input, specifies the length of the buffer pointed to by  <i>Buffer</i>, in bytes. If the buffer is large enough to contain all of the data, this function succeeds and <i>ReturnLength</i> is set to the number of bytes returned. If the buffer is not large enough to contain all of the data, the function fails, <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> returns ERROR_INSUFFICIENT_BUFFER, and <i>ReturnLength</i> is set to the buffer length required to contain all of the data. If the function fails with an error other than ERROR_INSUFFICIENT_BUFFER, the value of <i>ReturnLength</i> is undefined.


## -returns



If the function succeeds, the return value is TRUE and at least one <a href="https://msdn.microsoft.com/32ef5dd8-c00d-44ee-a291-a18653beb1b9">SYSTEM_LOGICAL_PROCESSOR_INFORMATION</a> structure is written to the output buffer.

If the function fails, the return value is FALSE. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



<b>GetLogicalProcessorInformation</b> can be used to get information about the relationship between logical processors in the system, including:

<ul>
<li>The logical processors that are part of a <a href="https://msdn.microsoft.com/a1263968-2b26-45cc-bdd7-6aa354821a5a">NUMA</a> node.</li>
<li>The logical processors that share resources. An example of this type of resource sharing would be hyperthreading scenarios.</li>
</ul>
Your application can use this information when affinitizing your threads and processes to take best advantage of the hardware properties of the platform, or to determine the number of logical and physical processors for licensing purposes.

Each of the <a href="https://msdn.microsoft.com/32ef5dd8-c00d-44ee-a291-a18653beb1b9">SYSTEM_LOGICAL_PROCESSOR_INFORMATION</a> structures returned in the buffer contains the following: 

<ul>
<li>A logical processor affinity mask, which indicates the logical processors that the information in the structure applies to.</li>
<li>A logical processor mask of type <a href="https://msdn.microsoft.com/2ada52f0-70ec-4146-9ef7-9af3b08996f9">LOGICAL_PROCESSOR_RELATIONSHIP</a>, which indicates the relationship between the logical processors in the mask. Applications calling this function must be prepared to handle additional indicator values in the future.</li>
</ul>
Note that the order in which the structures are returned in the buffer  may change between calls to this function.

The size of the <a href="https://msdn.microsoft.com/32ef5dd8-c00d-44ee-a291-a18653beb1b9">SYSTEM_LOGICAL_PROCESSOR_INFORMATION</a> structure varies between processor architectures and versions of Windows. For this reason, applications should first call this function to obtain the required buffer size, then dynamically allocate memory for the buffer.

On systems with more than 64 logical processors, the <b>GetLogicalProcessorInformation</b> function retrieves logical processor information about processors in the <a href="https://msdn.microsoft.com/c627ac0f-96e8-48b5-9103-4316f487e173">processor group</a> to which the calling thread is currently assigned. Use the <a href="https://msdn.microsoft.com/dfc4f444-4651-4a02-b8f6-f30d9278eae2">GetLogicalProcessorInformationEx</a> function to retrieve information about processors in all processor groups on the system.


#### Examples

The following C++ example uses the <b>GetLogicalProcessorInformation</b> function to display information about processors on the current system.  Because <b>GetLogicalProcessorInformation</b> is not present on all systems, this example uses the <a href="https://msdn.microsoft.com/a0d7fc09-f888-4f46-a571-d3719a627597">GetProcAddress</a> function instead of calling <b>GetLogicalProcessorInformation</b> directly.

This example reports the number of active processor cores. This example also reports the number of NUMA nodes, physical packages, and caches on systems that support this information.   For more information, see the description of the <b>Relationship</b> member of the <a href="https://msdn.microsoft.com/32ef5dd8-c00d-44ee-a291-a18653beb1b9">SYSTEM_LOGICAL_PROCESSOR_INFORMATION</a> structure. <b>Windows Server 2003, Windows XP Professional x64 Edition and Windows XP with SP3:  </b>This example reports the number of physical processors rather than the number of active processor cores. 




```cpp

#include <windows.h>
#include <malloc.h>    
#include <stdio.h>
#include <tchar.h>

typedef BOOL (WINAPI *LPFN_GLPI)(
    PSYSTEM_LOGICAL_PROCESSOR_INFORMATION, 
    PDWORD);


// Helper function to count set bits in the processor mask.
DWORD CountSetBits(ULONG_PTR bitMask)
{
    DWORD LSHIFT = sizeof(ULONG_PTR)*8 - 1;
    DWORD bitSetCount = 0;
    ULONG_PTR bitTest = (ULONG_PTR)1 << LSHIFT;    
    DWORD i;
    
    for (i = 0; i <= LSHIFT; ++i)
    {
        bitSetCount += ((bitMask & bitTest)?1:0);
        bitTest/=2;
    }

    return bitSetCount;
}

int _cdecl _tmain ()
{
    LPFN_GLPI glpi;
    BOOL done = FALSE;
    PSYSTEM_LOGICAL_PROCESSOR_INFORMATION buffer = NULL;
    PSYSTEM_LOGICAL_PROCESSOR_INFORMATION ptr = NULL;
    DWORD returnLength = 0;
    DWORD logicalProcessorCount = 0;
    DWORD numaNodeCount = 0;
    DWORD processorCoreCount = 0;
    DWORD processorL1CacheCount = 0;
    DWORD processorL2CacheCount = 0;
    DWORD processorL3CacheCount = 0;
    DWORD processorPackageCount = 0;
    DWORD byteOffset = 0;
    PCACHE_DESCRIPTOR Cache;

    glpi = (LPFN_GLPI) GetProcAddress(
                            GetModuleHandle(TEXT("kernel32")),
                            "GetLogicalProcessorInformation");
    if (NULL == glpi) 
    {
        _tprintf(TEXT("\nGetLogicalProcessorInformation is not supported.\n"));
        return (1);
    }

    while (!done)
    {
        DWORD rc = glpi(buffer, &returnLength);

        if (FALSE == rc) 
        {
            if (GetLastError() == ERROR_INSUFFICIENT_BUFFER) 
            {
                if (buffer) 
                    free(buffer);

                buffer = (PSYSTEM_LOGICAL_PROCESSOR_INFORMATION)malloc(
                        returnLength);

                if (NULL == buffer) 
                {
                    _tprintf(TEXT("\nError: Allocation failure\n"));
                    return (2);
                }
            } 
            else 
            {
                _tprintf(TEXT("\nError %d\n"), GetLastError());
                return (3);
            }
        } 
        else
        {
            done = TRUE;
        }
    }

    ptr = buffer;

    while (byteOffset + sizeof(SYSTEM_LOGICAL_PROCESSOR_INFORMATION) <= returnLength) 
    {
        switch (ptr->Relationship) 
        {
        case RelationNumaNode:
            // Non-NUMA systems report a single record of this type.
            numaNodeCount++;
            break;

        case RelationProcessorCore:
            processorCoreCount++;

            // A hyperthreaded core supplies more than one logical processor.
            logicalProcessorCount += CountSetBits(ptr->ProcessorMask);
            break;

        case RelationCache:
            // Cache data is in ptr->Cache, one CACHE_DESCRIPTOR structure for each cache. 
            Cache = &ptr->Cache;
            if (Cache->Level == 1)
            {
                processorL1CacheCount++;
            }
            else if (Cache->Level == 2)
            {
                processorL2CacheCount++;
            }
            else if (Cache->Level == 3)
            {
                processorL3CacheCount++;
            }
            break;

        case RelationProcessorPackage:
            // Logical processors share a physical package.
            processorPackageCount++;
            break;

        default:
            _tprintf(TEXT("\nError: Unsupported LOGICAL_PROCESSOR_RELATIONSHIP value.\n"));
            break;
        }
        byteOffset += sizeof(SYSTEM_LOGICAL_PROCESSOR_INFORMATION);
        ptr++;
    }

    _tprintf(TEXT("\nGetLogicalProcessorInformation results:\n"));
    _tprintf(TEXT("Number of NUMA nodes: %d\n"), 
             numaNodeCount);
    _tprintf(TEXT("Number of physical processor packages: %d\n"), 
             processorPackageCount);
    _tprintf(TEXT("Number of processor cores: %d\n"), 
             processorCoreCount);
    _tprintf(TEXT("Number of logical processors: %d\n"), 
             logicalProcessorCount);
    _tprintf(TEXT("Number of processor L1/L2/L3 caches: %d/%d/%d\n"), 
             processorL1CacheCount,
             processorL2CacheCount,
             processorL3CacheCount);
    
    free(buffer);

    return 0;
}


```





## -see-also




<a href="https://msdn.microsoft.com/dfc4f444-4651-4a02-b8f6-f30d9278eae2">GetLogicalProcessorInformationEx</a>



<a href="https://msdn.microsoft.com/2ada52f0-70ec-4146-9ef7-9af3b08996f9">LOGICAL_PROCESSOR_RELATIONSHIP</a>



<a href="https://msdn.microsoft.com/8c8e8af0-bf50-4a4b-945c-83bae1eff7dd">Process and Thread Functions</a>



<a href="https://msdn.microsoft.com/32ef5dd8-c00d-44ee-a291-a18653beb1b9">SYSTEM_LOGICAL_PROCESSOR_INFORMATION</a>
 

 
