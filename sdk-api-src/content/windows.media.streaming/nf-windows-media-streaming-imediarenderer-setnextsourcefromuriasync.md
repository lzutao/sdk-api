---
UID: NF:windows.media.streaming.IMediaRenderer.SetNextSourceFromUriAsync
title: IMediaRenderer::streaming
author: windows-sdk-content
description: Instructs the DMR asynchronously to prepare the content identified by the specified URI for playing once the current content has finished playing.
old-location: mediastreaming\imediarenderer_setnextsourcefromuriasync.htm
tech.root: mediastreaming
ms.assetid: 6894F1DF-63E2-4091-B61B-736D801E06EF
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMediaRenderer interface [Media Streaming API],SetNextSourceFromUriAsync method, IMediaRenderer.SetNextSourceFromUriAsync, IMediaRenderer.streaming, IMediaRenderer::SetNextSourceFromUriAsync, IMediaRenderer::streaming, SetNextSourceFromUriAsync, SetNextSourceFromUriAsync method [Media Streaming API], SetNextSourceFromUriAsync method [Media Streaming API],IMediaRenderer interface, mediastreaming.imediarenderer_setnextsourcefromuriasync, windows/IMediaRenderer::SetNextSourceFromUriAsync
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: windows.media.streaming.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - COM
api_location:
 - windows.media.streaming.h
api_name:
 - IMediaRenderer.SetNextSourceFromUriAsync
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMediaRenderer::streaming


## -description


Instructs the DMR asynchronously to prepare the content identified by the specified URI for playing once the current content has finished playing.


## -parameters




### -param URI [in]

An HSTRING containing the file path or resource location of media content.


### -param value [out]

Receives a reference to a <a href="https://msdn.microsoft.com/4899254A-C393-4D03-970F-CF272F4761B6">PlaybackOperation</a> object that is used to get results from the asynchronous operation.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

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
The method succeeded.

</td>
</tr>
</table>
 




## -remarks



Once the DMR finishes playing the current content, it will automatically switch to the content identified by the <i>URI</i> parameter.




## -see-also




<a href="https://msdn.microsoft.com/FBA5BF5A-FA5A-4E25-8F2B-9D1C0A9BCACB">IMediaRenderer</a>
 

 
