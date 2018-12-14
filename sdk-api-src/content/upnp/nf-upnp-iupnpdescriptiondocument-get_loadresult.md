---
UID: NF:upnp.IUPnPDescriptionDocument.get_LoadResult
title: IUPnPDescriptionDocument::get_LoadResult
author: windows-sdk-content
description: The LoadResult property specifies the success or failure code of a completed load operation.
old-location: upnp\iupnpdescriptiondocument_loadresult.htm
tech.root: upnp
ms.assetid: 3faf3dfa-ed42-4dbd-9ad7-7e34a8b00be8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: E_FAIL, E_PENDING, E_UNEXPECTED, IUPnPDescriptionDocument interface [UPnP APIs],get_LoadResult method, IUPnPDescriptionDocument.get_LoadResult, IUPnPDescriptionDocument::get_LoadResult, S_OK, _upnp_iupnpdescriptiondocument_loadresult, get_LoadResult, get_LoadResult method [UPnP APIs], get_LoadResult method [UPnP APIs],IUPnPDescriptionDocument interface, upnp.iupnpdescriptiondocument_loadresult, upnp/IUPnPDescriptionDocument::get_LoadResult
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: upnp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: None supported
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
req.dll: Upnp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Upnp.dll
api_name:
 - IUPnPDescriptionDocument.get_LoadResult
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUPnPDescriptionDocument::get_LoadResult


## -description


The 
<b>LoadResult</b> property specifies the success or failure code of a completed load operation.


## -parameters




### -param phrError [out]

Receives a reference to the success or failure code. The values this parameter can receive are:

<table>
<tr>
<th>phrError Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="E_FAIL"></a><a id="e_fail"></a><dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The load operation failed.

</td>
</tr>
<tr>
<td width="40%"><a id="E_PENDING"></a><a id="e_pending"></a><dl>
<dt><b>E_PENDING</b></dt>
</dl>
</td>
<td width="60%">
The load operation is not yet completed.

</td>
</tr>
<tr>
<td width="40%"><a id="E_UNEXPECTED"></a><a id="e_unexpected"></a><dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
An unexpected error occurred during the load operation.

</td>
</tr>
<tr>
<td width="40%"><a id="S_OK"></a><a id="s_ok"></a><dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The load operation succeeded.

</td>
</tr>
</table>
 


## -returns



For C++: If this property's "get" method succeeds, the return value is S_OK. Otherwise, the method returns one of the COM error codes defined in WinError.h.




## -remarks



This property specifies the error that the <a href="https://msdn.microsoft.com/02ae8af2-44f2-4b7c-a426-f2a26c43da37">IUPnPDescriptionDocument::Load</a> or <a href="https://msdn.microsoft.com/bfb1d833-13e8-4ffe-832d-f6640a42055a">IUPnPDescriptionDocument::LoadAsync</a> method generates. This property is useful when it is necessary to separate the load operation from the error checking.




## -see-also




<a href="https://msdn.microsoft.com/25bd3abd-b270-4609-93bb-a786ccaa95dd">IUPnPDescriptionDocument</a>



<a href="https://msdn.microsoft.com/02ae8af2-44f2-4b7c-a426-f2a26c43da37">IUPnPDescriptionDocument::Load</a>



<a href="https://msdn.microsoft.com/bfb1d833-13e8-4ffe-832d-f6640a42055a">IUPnPDescriptionDocument::LoadAsync</a>
 

 
