---
UID: NS:winnt._IMAGE_LOAD_CONFIG_DIRECTORY64
title: IMAGE_LOAD_CONFIG_DIRECTORY64
author: windows-sdk-content
description: Contains the load configuration data of an image.
old-location: base\image_load_config_directory64_str.htm
tech.root: debug
ms.assetid: ebd42f1a-a5aa-4179-a2d0-61c50469d5c0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PIMAGE_LOAD_CONFIG_DIRECTORY64, IMAGE_LOAD_CONFIG_DIRECTORY, IMAGE_LOAD_CONFIG_DIRECTORY32, IMAGE_LOAD_CONFIG_DIRECTORY64, IMAGE_LOAD_CONFIG_DIRECTORY64 structure, PIMAGE_LOAD_CONFIG_DIRECTORY64, PIMAGE_LOAD_CONFIG_DIRECTORY64 structure pointer, _IMAGE_LOAD_CONFIG_DIRECTORY64, base.image_load_config_directory64_str, winnt/IMAGE_LOAD_CONFIG_DIRECTORY64, winnt/PIMAGE_LOAD_CONFIG_DIRECTORY64"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winnt.h
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
 - WinNT.h
api_name:
 - IMAGE_LOAD_CONFIG_DIRECTORY64
 - IMAGE_LOAD_CONFIG_DIRECTORY
product: Windows
targetos: Windows
req.typenames: IMAGE_LOAD_CONFIG_DIRECTORY64, *PIMAGE_LOAD_CONFIG_DIRECTORY64
req.redist: 
---

# IMAGE_LOAD_CONFIG_DIRECTORY64 structure


## -description


Contains the load configuration data of an image.


## -struct-fields




### -field Size

The size of the structure. For Windows XP, the size must be specified as 64 for x86 images.


### -field TimeDateStamp

The date and time stamp value. The value is represented in the number of seconds elapsed since midnight (00:00:00), January 1, 1970, Universal Coordinated Time, according to the system clock. The time stamp can be printed using the C run-time (CRT) function <b>ctime</b>.


### -field MajorVersion

The major version number.


### -field MinorVersion

The minor version number.


### -field GlobalFlagsClear

The global flags that control system behavior. For more information, see Gflags.exe.


### -field GlobalFlagsSet

The global flags that control system behavior. For more information, see Gflags.exe.


### -field CriticalSectionDefaultTimeout

The critical section default time-out value.


### -field DeCommitFreeBlockThreshold

The size of the minimum block that must be freed before it is freed (de-committed), in bytes. This value is advisory.


### -field DeCommitTotalFreeThreshold

The size of the minimum total memory that must be freed in the process heap before it is freed (de-committed), in bytes. This value is advisory.


### -field LockPrefixTable

 The VA of a list of addresses where the LOCK prefix is used. These will be replaced by NOP on single-processor systems. This member is available only for x86.


### -field MaximumAllocationSize

The maximum allocation size, in bytes. This member is obsolete and is used only for debugging purposes.


### -field VirtualMemoryThreshold

The maximum block size that can be allocated from heap segments, in bytes.


### -field ProcessAffinityMask

The process affinity mask. For more information, see 
<a href="https://msdn.microsoft.com/f50ca86e-fa81-4ed9-ae6c-63a4e7f2a53f">GetProcessAffinityMask</a>. This member is available only for .exe files.


### -field ProcessHeapFlags

The process heap flags. For more information, see <a href="https://msdn.microsoft.com/8c0a77a2-37e6-41f7-bdc6-1f3768d61c9b">HeapCreate</a>.


### -field CSDVersion

The service pack version.


### -field DependentLoadFlags

 


### -field EditList

Reserved for use by the system.


### -field SecurityCookie

A pointer to a cookie that is used by Visual C++ or GS implementation.


### -field SEHandlerTable

 The VA of the sorted table of RVAs of each valid, unique handler in the image. This member is available only for x86.


### -field SEHandlerCount

The count of unique handlers in the table. This member is available only for x86.


### -field GuardCFCheckFunctionPointer

 


### -field GuardCFDispatchFunctionPointer

 


### -field GuardCFFunctionTable

 


### -field GuardCFFunctionCount

 


### -field GuardFlags

 


### -field CodeIntegrity

 


### -field GuardAddressTakenIatEntryTable

 


### -field GuardAddressTakenIatEntryCount

 


### -field GuardLongJumpTargetTable

 


### -field GuardLongJumpTargetCount

 


### -field DynamicValueRelocTable

 


### -field CHPEMetadataPointer

 


### -field GuardRFFailureRoutine

 


### -field GuardRFFailureRoutineFunctionPointer

 


### -field DynamicValueRelocTableOffset

 


### -field DynamicValueRelocTableSection

 


### -field Reserved2

 


### -field GuardRFVerifyStackPointerFunctionPointer

 


### -field HotPatchTableOffset

 


### -field Reserved3

 


### -field EnclaveConfigurationPointer

 


### -field VolatileMetadataPointer

 




#### - Reserved1

Reserved for use by the operating system.


## -remarks



If <b>_WIN64</b> is defined, then <b>IMAGE_LOAD_CONFIG_DIRECTORY</b> is defined as <b>IMAGE_LOAD_CONFIG_DIRECTORY64</b>. However, if <b>_WIN64</b> is not defined,  then <b>IMAGE_LOAD_CONFIG_DIRECTORY</b> is defined as <b>IMAGE_LOAD_CONFIG_DIRECTORY32</b>. 

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>typedef struct {
    DWORD   Size;
    DWORD   TimeDateStamp;
    WORD    MajorVersion;
    WORD    MinorVersion;
    DWORD   GlobalFlagsClear;
    DWORD   GlobalFlagsSet;
    DWORD   CriticalSectionDefaultTimeout;
    DWORD   DeCommitFreeBlockThreshold;
    DWORD   DeCommitTotalFreeThreshold;
    DWORD   LockPrefixTable;            // VA
    DWORD   MaximumAllocationSize;
    DWORD   VirtualMemoryThreshold;
    DWORD   ProcessHeapFlags;
    DWORD   ProcessAffinityMask;
    WORD    CSDVersion;
    WORD    Reserved1;
    DWORD   EditList;                   // VA
    DWORD   SecurityCookie;             // VA
    DWORD   SEHandlerTable;             // VA
    DWORD   SEHandlerCount;
} IMAGE_LOAD_CONFIG_DIRECTORY32, *PIMAGE_LOAD_CONFIG_DIRECTORY32;</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/5d9b6705-7e65-4a60-912e-8ffcff9d7921">GetImageConfigInformation</a>



<a href="https://msdn.microsoft.com/f50ca86e-fa81-4ed9-ae6c-63a4e7f2a53f">GetProcessAffinityMask</a>



<a href="https://msdn.microsoft.com/b88c7a21-933f-450c-97e8-04cf3c5f9b11">ImageHlp Structures</a>



<a href="https://msdn.microsoft.com/396af0c0-2fb1-418b-bc2b-9e9eb63174bc">SetImageConfigInformation</a>
 

 
