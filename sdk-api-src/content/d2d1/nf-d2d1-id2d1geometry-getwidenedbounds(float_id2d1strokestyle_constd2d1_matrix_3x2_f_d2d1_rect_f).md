---
UID: NF:d2d1.ID2D1Geometry.GetWidenedBounds(FLOAT,ID2D1StrokeStyle,const D2D1_MATRIX_3X2_F,D2D1_RECT_F)
title: ID2D1Geometry::GetWidenedBounds(FLOAT,ID2D1StrokeStyle,const D2D1_MATRIX_3X2_F,D2D1_RECT_F)
author: windows-sdk-content
description: Gets the bounds of the geometry after it has been widened by the specified stroke width and style and transformed by the specified matrix.
old-location: direct2d\ID2D1Geometry_GetWidenedBounds_FLOAT_ptr_ID2D1StrokeStyle_ptr_D2D_MATRIX_3X2_F_ptr_D2D_RECT_F.htm
tech.root: direct2d
ms.assetid: 3cca4272-fa42-4849-9e85-9dcec39531ec
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetWidenedBounds, GetWidenedBounds method [Direct2D], GetWidenedBounds method [Direct2D],ID2D1Geometry interface, ID2D1Geometry interface [Direct2D],GetWidenedBounds method, ID2D1Geometry.GetWidenedBounds, ID2D1Geometry.GetWidenedBounds(FLOAT,ID2D1StrokeStyle,const D2D1_MATRIX_3X2_F,D2D1_RECT_F), ID2D1Geometry::GetWidenedBounds, ID2D1Geometry::GetWidenedBounds(FLOAT,ID2D1StrokeStyle,const D2D1_MATRIX_3X2_F,D2D1_RECT_F), d2d1/ID2D1Geometry::GetWidenedBounds, direct2d.ID2D1Geometry_GetWidenedBounds_FLOAT_ptr_ID2D1StrokeStyle_ptr_D2D_MATRIX_3X2_F_ptr_D2D_RECT_F
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d2d1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D2d1.lib
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
 - ID2D1Geometry.GetWidenedBounds
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1Geometry::GetWidenedBounds(FLOAT,ID2D1StrokeStyle,const D2D1_MATRIX_3X2_F,D2D1_RECT_F)


## -description


Gets the bounds of the geometry after it has been widened by the specified stroke width and style and transformed by the specified matrix.


## -parameters




### -param strokeWidth

Type: <b>FLOAT</b>

The amount by which to widen the geometry by stroking its outline.


### -param strokeStyle [in, optional]

Type: <b><a href="https://msdn.microsoft.com/2cdf66dc-f34f-4132-8c06-7464648d3cef">ID2D1StrokeStyle</a>*</b>

The style of the stroke that widens the geometry.



### -param worldTransform [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/f05d7555-6482-4eea-950f-7b443892cc1f">D2D1_MATRIX_3X2_F</a>*</b>

A transform to apply to the geometry after the geometry is transformed and after the geometry has been stroked, or <b>NULL</b>.


### -param bounds [out]

Type: <b><a href="https://msdn.microsoft.com/a961c0e3-fb76-4c07-b76e-47d8c09ada08">D2D1_RECT_F</a>*</b>

When this method returns, contains the bounds of the widened geometry. You must allocate storage for this parameter.


## -returns



Type: <b><a href="a9046ed2-bfb2-4d56-a719-2824afce59ac">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/be4ab801-64f6-48f9-8f62-d0492cc438b1">ID2D1Geometry</a>
 

 
