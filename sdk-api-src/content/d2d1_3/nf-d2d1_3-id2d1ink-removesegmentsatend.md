---
UID: NF:d2d1_3.ID2D1Ink.RemoveSegmentsAtEnd
title: ID2D1Ink::RemoveSegmentsAtEnd
author: windows-sdk-content
description: Removes the given number of segments from the end of this ink object.
old-location: direct2d\id2d1ink_removesegmentsatend.htm
tech.root: direct2d
ms.assetid: 8EA09675-971E-4399-B718-E7433D894867
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID2D1Ink interface [Direct2D],RemoveSegmentsAtEnd method, ID2D1Ink.RemoveSegmentsAtEnd, ID2D1Ink::RemoveSegmentsAtEnd, RemoveSegmentsAtEnd, RemoveSegmentsAtEnd method [Direct2D], RemoveSegmentsAtEnd method [Direct2D],ID2D1Ink interface, d2d1_3/ID2D1Ink::RemoveSegmentsAtEnd, direct2d.id2d1ink_removesegmentsatend
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d2d1_3.h
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
req.lib: D2d1_3.lib
req.dll: D2d1_3.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - d2d1_3.dll
api_name:
 - ID2D1Ink.RemoveSegmentsAtEnd
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1Ink::RemoveSegmentsAtEnd


## -description


Removes the given number of segments from the end of this ink object.


## -parameters




### -param segmentsCount

Type: <b>UINT32</b>

The number of segments to be removed from the end of this ink object. Note that segmentsCount must be less or equal to the number of segments in the ink object.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/4B6DD4C2-8E91-4AEA-AFB5-21B4FD13F75A">ID2D1Ink</a>
 

 
