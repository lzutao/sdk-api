---
UID: NS:vdssys._MERGE_VIRTUAL_DISK_PARAMETERS
title: "_MERGE_VIRTUAL_DISK_PARAMETERS"
author: windows-sdk-content
description: Contains virtual hard disk (VHD) merge request parameters.
old-location: vhd\merge_virtual_disk_parameters.htm
old-project: VStor
ms.assetid: 5bb84e11-677d-42f5-b5b6-59f23b9a8ab7
ms.author: windowssdkdev
ms.date: 05/29/2018
ms.keywords: "*PMERGE_VIRTUAL_DISK_PARAMETERS, MERGE_VIRTUAL_DISK_PARAMETERS, MERGE_VIRTUAL_DISK_PARAMETERS structure [VHD], PMERGE_VIRTUAL_DISK_PARAMETERS, PMERGE_VIRTUAL_DISK_PARAMETERS structure pointer [VHD], _MERGE_VIRTUAL_DISK_PARAMETERS, vdssys/MERGE_VIRTUAL_DISK_PARAMETERS, vdssys/PMERGE_VIRTUAL_DISK_PARAMETERS, vhd.merge_virtual_disk_parameters, virtdisk/MERGE_VIRTUAL_DISK_PARAMETERS, virtdisk/PMERGE_VIRTUAL_DISK_PARAMETERS"
ms.prod: windows
ms.technology: windows-sdk
ms.topic: struct
req.header: vdssys.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7
req.target-min-winversvr: Windows Server 2008 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
tech.root: 
req.typenames: MERGE_VIRTUAL_DISK_PARAMETERS, *PMERGE_VIRTUAL_DISK_PARAMETERS
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - VirtDisk.h
 - vdssys.h
api_name:
 - MERGE_VIRTUAL_DISK_PARAMETERS
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Windows UI
---

# _MERGE_VIRTUAL_DISK_PARAMETERS structure


## -description


Contains virtual hard disk (VHD) merge request parameters.


## -struct-fields




### -field Version

A <a href="https://msdn.microsoft.com/1f542a51-d314-4add-a389-d450785b0a73">MERGE_VIRTUAL_DISK_VERSION</a> enumeration 
      that specifies the version of the 
      <b>MERGE_VIRTUAL_DISK_PARAMETERS</b> structure 
      being passed to or from the VHD functions.


### -field Version1

This structure is used when the Version member is <b>MERGE_VIRTUAL_DISK_VERSION_1</b> 
       (1).


### -field Version1.MergeDepth

Depth of the merge request. This is the number of parent disks in the differencing chain to merge 
         together.

<div class="alert"><b>Note</b>  The RWDepth of the virtual disk must be greater than <b>MergeDepth</b>. For more 
         information, see 
         <a href="https://msdn.microsoft.com/ad67bc3e-a0fe-4198-9307-819577abef7f">OPEN_VIRTUAL_DISK_PARAMETERS</a>.</div>
<div> </div>

### -field Version2

This structure is used when the Version member is <b>MERGE_VIRTUAL_DISK_VERSION_2</b> 
        (2).

<b>Windows 7 and Windows Server 2008 R2:  </b>This value is not supported until Windows 8 and Windows Server 2012.


### -field Version2.MergeSourceDepth

Depth from the leaf from which to begin the merge.  The leaf is at depth 1.


### -field Version2.MergeTargetDepth

Depth from  the leaf to target the merge.  The leaf is at depth 1.


## -remarks



The depth of a merge request specified by the <b>MergeDepth</b> member is the number of  
    parent VHD image files in the differencing chain to be merged.  For more information, see 
    <a href="https://msdn.microsoft.com/9a9068d1-2f81-42a2-a3b2-6030a24a4445">MergeVirtualDisk</a>.




## -see-also




<a href="https://msdn.microsoft.com/c9531c07-ad55-42b6-8685-7f55a47e8485">About VHD</a>



<a href="https://msdn.microsoft.com/9a9068d1-2f81-42a2-a3b2-6030a24a4445">MergeVirtualDisk</a>



<a href="https://msdn.microsoft.com/3b5d0da0-2b23-4b7c-b007-ed3fe030926c">VHD Reference</a>
 

 
