---
UID: NF:gdiplusheaders.Region.Intersect(IN const RectF &)
title: Region::Intersect(IN const RectF &)
author: windows-sdk-content
description: The Region::Intersect method updates this region to the portion of itself that intersects the specified rectangle's interior.
old-location: gdiplus\_gdiplus_CLASS_Region_Intersect_RectF_rect_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\regionclass\regionmethods\regionintersectmethods\intersect_38rectfamprect.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Intersect, Intersect method [GDI+], Intersect method [GDI+],Region class, Region class [GDI+],Intersect method, Region.Intersect, Region.Intersect(IN const RectF &), Region.Intersect(const RectF&), Region::Intersect, Region::Intersect(IN const RectF &), _gdiplus_CLASS_Region_Intersect_RectF_rect_, gdiplus._gdiplus_CLASS_Region_Intersect_RectF_rect_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusheaders.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gdiplus.dll
api_name:
 - Region.Intersect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Region::Intersect(IN const RectF &)


## -description


The <b>Region::Intersect</b> method updates this region to the portion of itself that intersects the specified rectangle's interior.


## -parameters




### -param rect [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/6821442b-d352-48cb-a48a-839105a8c36a">RectF</a></b>

Reference to a rectangle to use to update this 
					<a href="https://msdn.microsoft.com/2972b879-7d2f-4cad-b17d-670125f43691">Region</a>object. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns <b>Ok</b>, which is an element of the 
<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/9b995615-3ea1-488d-8960-90add719c3f9">Rect</a>



<a href="https://msdn.microsoft.com/2972b879-7d2f-4cad-b17d-670125f43691">Region</a>



<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a>
 

 
