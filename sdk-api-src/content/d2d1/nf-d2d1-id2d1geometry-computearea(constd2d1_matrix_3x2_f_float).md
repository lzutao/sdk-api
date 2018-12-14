---
UID: NF:d2d1.ID2D1Geometry.ComputeArea(const D2D1_MATRIX_3X2_F,FLOAT)
title: ID2D1Geometry::ComputeArea(const D2D1_MATRIX_3X2_F,FLOAT)
author: windows-sdk-content
description: Computes the area of the geometry after it has been transformed by the specified matrix and flattened using the specified tolerance.
old-location: direct2d\ID2D1Geometry_ComputeArea_ptr_D2D_MATRIX_3X2_F_FLOAT_ptr_FLOAT.htm
tech.root: direct2d
ms.assetid: 1efc99d7-453f-4c51-a523-00c38fa00ff4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ComputeArea, ComputeArea method [Direct2D], ComputeArea method [Direct2D],ID2D1Geometry interface, ID2D1Geometry interface [Direct2D],ComputeArea method, ID2D1Geometry.ComputeArea, ID2D1Geometry.ComputeArea(const D2D1_MATRIX_3X2_F,FLOAT), ID2D1Geometry::ComputeArea, ID2D1Geometry::ComputeArea(const D2D1_MATRIX_3X2_F,FLOAT), ID2D1Geometry::ComputeArea,ID2D1Geometry::ComputeArea(const D2D1_MATRIX_3X2_F,FLOAT,FLOAT), d2d1/ID2D1Geometry::ComputeArea, direct2d.ID2D1Geometry_ComputeArea_ptr_D2D_MATRIX_3X2_F_FLOAT_ptr_FLOAT
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
 - ID2D1Geometry.ComputeArea
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1Geometry::ComputeArea(const D2D1_MATRIX_3X2_F,FLOAT)


## -description


Computes the area of the geometry after it has been transformed by the specified matrix and flattened using the specified tolerance.


## -parameters




### -param worldTransform [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/f05d7555-6482-4eea-950f-7b443892cc1f">D2D1_MATRIX_3X2_F</a>*</b>

The transform to apply to this geometry before computing its area, or <b>NULL</b>.


### -param area [out]

Type: <b>FLOAT*</b>

When this this method returns, contains a pointer to the area of the transformed, flattened version of this geometry. You must allocate storage for this parameter.


#### - flatteningTolerance

Type: <b>FLOAT</b>

The maximum error allowed when constructing a polygonal approximation of the geometry. No point in the polygonal representation will diverge from the original geometry by more than the flattening tolerance. Smaller values produce more accurate results but cause slower execution. 



## -returns



Type: <b><a href="a9046ed2-bfb2-4d56-a719-2824afce59ac">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/be4ab801-64f6-48f9-8f62-d0492cc438b1">ID2D1Geometry</a>
 

 
