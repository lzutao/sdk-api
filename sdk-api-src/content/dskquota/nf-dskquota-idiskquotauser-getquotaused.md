---
UID: NF:dskquota.IDiskQuotaUser.GetQuotaUsed
title: IDiskQuotaUser::GetQuotaUsed
author: windows-sdk-content
description: Retrieves the user's quota used value on the volume.
old-location: fs\idiskquotauser_getquotaused.htm
tech.root: fileio
ms.assetid: 3787648e-7788-4d09-a236-fe28a693a8ff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetQuotaUsed, GetQuotaUsed method [Files], GetQuotaUsed method [Files],IDiskQuotaUser interface, IDiskQuotaUser interface [Files],GetQuotaUsed method, IDiskQuotaUser.GetQuotaUsed, IDiskQuotaUser::GetQuotaUsed, _win32_idiskquotauser_getquotaused, base.idiskquotauser_getquotaused, dskquota/IDiskQuotaUser::GetQuotaUsed, fs.idiskquotauser_getquotaused
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
 - IDiskQuotaUser.GetQuotaUsed
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDiskQuotaUser::GetQuotaUsed


## -description


Retrieves the user's quota used value on the volume. This is the amount of information stored on the volume by the user. This is the amount of uncompressed information. Therefore, the use of NTFS file system compression does not affect this value.


## -parameters




### -param pllUsed [out]

The quota used value.


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
<dt><b>ERROR_LOCK_FAILED</b></dt>
</dl>
</td>
<td width="60%">
Failure to obtain an exclusive lock.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>pllUsed</i> parameter is <b>NULL</b>.

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
 




## -see-also




<a href="https://msdn.microsoft.com/c1f79e2e-834b-41dc-a15f-6dd1034d021b">Disk Management Interfaces</a>



<a href="https://msdn.microsoft.com/42efbd5b-6455-4319-a76e-cdb666fc36b8">Disk Quotas</a>



<a href="https://msdn.microsoft.com/27edbebc-35b4-4f6a-87cc-d8a99782f405">IDiskQuotaUser</a>
 

 
