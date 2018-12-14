---
UID: NF:resapi.ClusterGetVolumePathName
title: ClusterGetVolumePathName function
author: windows-sdk-content
description: ClusterGetVolumePathName may be altered or unavailable. Instead, use GetVolumePathName.
old-location: mscs\clustergetvolumepathname.htm
tech.root: mscs
ms.assetid: eff2995a-d17c-4899-bff5-ead9526f859d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ClusterGetVolumePathName, ClusterGetVolumePathName function [Failover Cluster], PCLUSTER_GET_VOLUME_PATH_NAME, PCLUSTER_GET_VOLUME_PATH_NAME function [Failover Cluster], mscs.clustergetvolumepathname, resapi/ClusterGetVolumePathName, resapi/PCLUSTER_GET_VOLUME_PATH_NAME
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: resapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2 Enterprise, Windows Server 2008 R2 Datacenter
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: ResUtils.Lib
req.dll: ResUtils.Dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - ResUtils.Dll
 - Ext-MS-Win-Cluster-ResUtils-l1-1-0.dll
 - ext-ms-win-cluster-resutils-l1-1-1.dll
api_name:
 - ClusterGetVolumePathName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterGetVolumePathName function


## -description


<p class="CCE_Message">[<b>ClusterGetVolumePathName</b> is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions. Instead, use <a href="https://msdn.microsoft.com/fa34786c-af82-4b59-bf36-e9a95a2f913e">GetVolumePathName</a>.]

Retrieves the volume mount point on the cluster where the specified path is mounted.


## -parameters




### -param lpszFileName [in]

A pointer to the input path string. Both absolute and relative file and directory names, for example 
       "..", are acceptable in this path.

If you specify a relative directory or file name without a volume qualifier, 
       <b>ClusterGetVolumePathName</b> returns the drive letter of the 
       current volume.

If this parameter is an empty string, "", the function fails but the last error is set to 
       <b>ERROR_SUCCESS</b>.


### -param lpszVolumePathName [out]

A pointer to a string that receives the volume mount point for the input path.


### -param cchBufferLength [in]

The length of the output buffer, in <b>WCHARs</b>.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call 
       <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The following examples may help. In these examples "Filename.Ext" does exist but 
     "Path\that\does\not\exist" does not.

<ul>
<li>
Input: "C:\ClusterStorage\Volume31\Filename.Ext"

Output: "C:\ClusterStorage\Volume31\"

</li>
<li>
Input: "\\?\C:\ClusterStorage\Volume31\Filename.Ext"

Output: "\\?\C:\ClusterStorage\Volume31\"

</li>
<li>
Input: "C:\ClusterStorage\Volume31\Path\that\does\not\exist"

Output: "C:\ClusterStorage\Volume31\"

</li>
<li>
Input: 
       "\\?\Volume{deadbeef-895e-4a1d-9d64-9b82fa068d76}\ClusterStorage\Volume31\Filename.Ext"

Output: "\\?\Volume{deadbeef-895e-4a1d-9d64-9b82fa068d76}\ClusterStorage\Volume31\"

</li>
<li>
Input: 
       "\\?\GLOBALROOT\Device\Harddisk0\Partition1\ClusterStorage\Volume31\Filename.Ext"

Output: "\\?\GLOBALROOT\Device\Harddisk0\Partition1\ClusterStorage\Volume31\"

</li>
<li>
Input: 
       "\\?\GLOBALROOT\Device\HarddiskVolume1\ClusterStorage\Volume31\Filename.Ext"

Output: "\\?\GLOBALROOT\Device\HarddiskVolume1\ClusterStorage\Volume31\"

</li>
</ul>
<b>Windows Server 2008 R2:  </b>The initial release of ResApi.h containing the 
      <b>ClusterGetVolumePathName</b> function used 
      <b>TCHAR</b>-based data types instead of <b>WCHAR</b>-based 
      data types. The UNICODE preprocessor define must be set before ResApi.h is included.


```cpp
#define UNICODE 1
#include <ResApi.h>
```




The 
    <b>ClusterGetVolumePathName</b> 
    function must be called from a node of the cluster.




## -see-also




<a href="https://msdn.microsoft.com/ea8b76b2-3931-4489-a648-e1077fd93b21">Backing Up and Restoring the Failover Cluster Configuration Using VSS</a>



<a href="https://msdn.microsoft.com/0f492e51-f364-40f1-b2c8-478f707f079d">Backup and Restore Functions</a>
 

 
