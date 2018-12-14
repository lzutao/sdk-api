---
UID: NF:d2d1_1.ID2D1CommandSink.SetTags
title: ID2D1CommandSink::SetTags
author: windows-sdk-content
description: Sets the tags that correspond to the tags in the command sink.
old-location: direct2d\id2d1commandsink_settags.htm
tech.root: direct2d
ms.assetid: 56898541-8c4a-4dbb-aa34-cc957b1f17ff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID2D1CommandSink interface [Direct2D],SetTags method, ID2D1CommandSink.SetTags, ID2D1CommandSink::SetTags, SetTags, SetTags method [Direct2D], SetTags method [Direct2D],ID2D1CommandSink interface, d2d1_1/ID2D1CommandSink::SetTags, direct2d.id2d1commandsink_settags
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d2d1_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
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
req.dll: D2d1.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D2d1.dll
api_name:
 - ID2D1CommandSink.SetTags
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1CommandSink::SetTags


## -description


Sets the tags that correspond to the tags in the command sink.


## -parameters




### -param tag1

Type: <b><a href="https://msdn.microsoft.com/4f363295-f140-4149-ba78-3abbc56eebe8">D2D1_TAG</a></b>

The first tag to associate with the primitive.


### -param tag2

Type: <b><a href="https://msdn.microsoft.com/4f363295-f140-4149-ba78-3abbc56eebe8">D2D1_TAG</a></b>

The second tag to associate with the primitive.


## -returns



Type: <b>HRESULT</b>

If the method succeeds, it returns <b>S_OK</b>. If it fails, it returns an <b>HRESULT</b> error code. 





## -see-also




<a href="https://msdn.microsoft.com/52e6da86-c7c6-48e7-b0ff-a54770663f14">ID2D1CommandList::Stream</a>



<a href="https://msdn.microsoft.com/4e0ce837-7f4e-4b93-8dd7-68f60cfb1105">ID2D1CommandSink</a>



<a href="https://msdn.microsoft.com/d71c3500-e11f-4b2d-9b78-b57df7dbc2bd">ID2D1RenderTarget::SetTags</a>
 

 
