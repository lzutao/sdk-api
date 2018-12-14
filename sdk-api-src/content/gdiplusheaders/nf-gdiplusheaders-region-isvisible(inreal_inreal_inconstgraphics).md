---
UID: NF:gdiplusheaders.Region.IsVisible(IN REAL,IN REAL,IN const Graphics)
title: Region::IsVisible(IN REAL,IN REAL,IN const Graphics)
author: windows-sdk-content
description: The Region::IsVisible method determines whether a point is inside this region.
old-location: gdiplus\_gdiplus_CLASS_Region_IsVisible_REAL_x_REAL_y_Graphics_g_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\regionclass\regionmethods\regionisvisiblemethods\isvisible_52realx_realy_graphicsg.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IsVisible, IsVisible method [GDI+], IsVisible method [GDI+],Region class, Region class [GDI+],IsVisible method, Region.IsVisible, Region.IsVisible(IN REAL,IN REAL,IN const Graphics), Region.IsVisible(REAL,REAL,const Graphics*), Region::IsVisible, Region::IsVisible(IN REAL,IN REAL,IN const Graphics), _gdiplus_CLASS_Region_IsVisible_REAL_x_REAL_y_Graphics_g_, gdiplus._gdiplus_CLASS_Region_IsVisible_REAL_x_REAL_y_Graphics_g_
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
 - Region.IsVisible
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# Region::IsVisible(IN REAL,IN REAL,IN const Graphics)


## -description


The <b>Region::IsVisible</b> method determines whether a point is inside this region.


## -parameters




### -param x [in]

Type: <b>REAL</b>

Real number that specifies the x-coordinate of the point to test. 


### -param y [in]

Type: <b>REAL</b>

Real number that specifies the y-coordinate of the point to test. 


### -param g [in]

Type: <b>const <a href="https://msdn.microsoft.com/7e874710-3cd3-42c8-bd2f-8a779b19ba59">Graphics</a>*</b>

Optional. Pointer to a <a href="https://msdn.microsoft.com/7e874710-3cd3-42c8-bd2f-8a779b19ba59">Graphics</a> object that contains the world and page transformations required to calculate the device coordinates of this region and the point. The default value is <b>NULL</b>. 


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the point is inside this region, this method returns <b>TRUE</b>; otherwise, it returns <b>FALSE</b>.




## -remarks



<div class="alert"><b>Note</b>  A region contains its border.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/7e874710-3cd3-42c8-bd2f-8a779b19ba59">Graphics</a>



<a href="https://msdn.microsoft.com/9b995615-3ea1-488d-8960-90add719c3f9">Rect</a>



<a href="https://msdn.microsoft.com/2972b879-7d2f-4cad-b17d-670125f43691">Region</a>
 

 
