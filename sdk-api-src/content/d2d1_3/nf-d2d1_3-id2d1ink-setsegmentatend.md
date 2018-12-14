---
UID: NF:d2d1_3.ID2D1Ink.SetSegmentAtEnd
title: ID2D1Ink::SetSegmentAtEnd
author: windows-sdk-content
description: Updates the last segment in this ink object with new control points.
old-location: direct2d\id2d1ink_setsegmentatend.htm
tech.root: direct2d
ms.assetid: E80083E4-7BBB-4AF5-81EB-49E68D6521F7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID2D1Ink interface [Direct2D],SetSegmentAtEnd method, ID2D1Ink.SetSegmentAtEnd, ID2D1Ink::SetSegmentAtEnd, ID2D1Ink::SetSegmentAtEnd(const D2D1_INK_BEZIER_SEGMENT), SetSegmentAtEnd, SetSegmentAtEnd method [Direct2D], SetSegmentAtEnd method [Direct2D],ID2D1Ink interface, d2d1_3/ID2D1Ink::SetSegmentAtEnd, direct2d.id2d1ink_setsegmentatend
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
 - ID2D1Ink.SetSegmentAtEnd
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1Ink::SetSegmentAtEnd


## -description


Updates the last segment in this ink object with new control points.


## -parameters




### -param segment [in]

Type: <b>const <a href="https://msdn.microsoft.com/27F1F78B-2478-4F5D-BF56-9931E767C358">D2D1_INK_BEZIER_SEGMENT</a>*</b>

A pointer to the segment data with which to overwrite this ink object's last segment. Note that if there are currently no segments in the ink object, SetSegmentsAtEnd will return an error.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/4B6DD4C2-8E91-4AEA-AFB5-21B4FD13F75A">ID2D1Ink</a>
 

 
