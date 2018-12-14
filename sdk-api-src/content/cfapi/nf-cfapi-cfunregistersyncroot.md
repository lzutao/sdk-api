---
UID: NF:cfapi.CfUnregisterSyncRoot
title: CfUnregisterSyncRoot function
author: windows-sdk-content
description: Unregisters a previously registered sync root.
old-location: cloudapi\cfunregistersyncroot.htm
tech.root: cfApi
ms.assetid: B4DA85DB-A63A-45EB-9F71-9395AC026A0C
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CfUnregisterSyncRoot, CfUnregisterSyncRoot function, cfapi/CfUnregisterSyncRoot, cloudApi.cfunregistersyncroot
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1709 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: CldApi.lib
req.dll: CldApi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - CldApi.dll
api_name:
 - CfUnregisterSyncRoot
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CfUnregisterSyncRoot function


## -description


Unregisters a previously registered sync root.


## -parameters




### -param SyncRootPath [in]

The path to the sync root to be unregistered.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Unregisters a sync root that was registered with <a href="https://msdn.microsoft.com/FAD56873-8812-42DC-9975-9507F73BD9E3">CfRegisterSyncRoot</a>. This is typically called at the sync provider uninstall time, when a user account is deleted, or when a user opts to no longer sync a directory tree (if supported by the sync provider). 

The sync provider should have WRITE_DATA or WRITE_DAC access to the sync root to be unregistered, or  unregistration will fail with: HRESULT(ERROR_CLOUD_FILE_ACCESS_DENIED).

Unregisters a sync root by traversing the directory tree of the sync root. 


For placeholder files:

<ul>
<li>If a placeholder file is fully hydrated, it is reverted back to a "normal" file. </li>
<li>If a placeholder file is not hydrated, it is permanently deleted from the local machine. </li>
</ul>
For placeholder directories:

<ul>
<li>If a placeholder directory is fully populated, it is reverted back to a "normal" directory.</li>
<li>If a placeholder directory is not fully populated, the directory is permanently deleted from the local machine.</li>
</ul>



<div class="alert"><b>Note</b>  If the placeholder files or directories cannot be reverted or deleted, it will be skipped, and the unregistering process will continue until the full sync root tree has been traversed.</div>
<div> </div>



