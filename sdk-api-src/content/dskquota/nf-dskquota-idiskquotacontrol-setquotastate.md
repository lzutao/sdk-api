---
UID: NF:dskquota.IDiskQuotaControl.SetQuotaState
title: IDiskQuotaControl::SetQuotaState
author: windows-sdk-content
description: Sets the state of the quota system.
old-location: fs\idiskquotacontrol_setquotastate.htm
tech.root: fileio
ms.assetid: 0bbacc3c-e212-4801-95d8-1e260123665d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDiskQuotaControl interface [Files],SetQuotaState method, IDiskQuotaControl.SetQuotaState, IDiskQuotaControl::SetQuotaState, SetQuotaState, SetQuotaState method [Files], SetQuotaState method [Files],IDiskQuotaControl interface, _win32_idiskquotacontrol_setquotastate, base.idiskquotacontrol_setquotastate, dskquota/IDiskQuotaControl::SetQuotaState, fs.idiskquotacontrol_setquotastate
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dskquota.h
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
req.lib: 
req.dll: Dskquota.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dskquota.dll
api_name:
 - IDiskQuotaControl.SetQuotaState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDiskQuotaControl::SetQuotaState


## -description


Sets the state of the quota system.


## -parameters




### -param dwState [in]

State to be applied to the volume. Use the following macros to set the proper bits.
					

<table>
<tr>
<th>Macro</th>
<th>Enable</th>
<th>Track</th>
<th>Enforce</th>
</tr>
<tr>
<td>DISKQUOTA_SET_DISABLED</td>
<td>No</td>
<td>No</td>
<td>No</td>
</tr>
<tr>
<td>DISKQUOTA_SET_TRACKED</td>
<td>Yes</td>
<td>Yes</td>
<td>No</td>
</tr>
<tr>
<td>DISKQUOTA_SET_ENFORCED</td>
<td>Yes</td>
<td>Yes</td>
<td>Yes</td>
</tr>
</table>
 


## -returns



This method returns a file system error or one of the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
The caller has insufficient access rights.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_READY</b></dt>
</dl>
</td>
<td width="60%">
The <b>DiskQuotaControl</b> object is not initialized.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>dwState</i> parameter is incorrect.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
An unexpected file system error occurred.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
An unexpected exception occurred.

</td>
</tr>
</table>
 




## -remarks



Not all state attributes can be modified. The enable, track, and enforce attributes can be modified.




## -see-also




<a href="https://msdn.microsoft.com/c1f79e2e-834b-41dc-a15f-6dd1034d021b">Disk Management Interfaces</a>



<a href="https://msdn.microsoft.com/42efbd5b-6455-4319-a76e-cdb666fc36b8">Disk Quotas</a>



<a href="https://msdn.microsoft.com/fc9add5a-c9ef-462d-8125-128d48018717">IDiskQuotaControl</a>
 

 
