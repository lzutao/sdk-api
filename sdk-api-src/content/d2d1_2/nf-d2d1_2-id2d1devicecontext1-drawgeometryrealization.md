---
UID: NF:d2d1_2.ID2D1DeviceContext1.DrawGeometryRealization
title: ID2D1DeviceContext1::DrawGeometryRealization
author: windows-sdk-content
description: Renders a given geometry realization to the target with the specified brush.
old-location: direct2d\id2d1devicecontext1_drawgeometryrealization.htm
tech.root: direct2d
ms.assetid: BA4FB8E7-E59A-42BD-86BB-8048267A26AA
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DrawGeometryRealization, DrawGeometryRealization method [Direct2D], DrawGeometryRealization method [Direct2D],ID2D1DeviceContext1 interface, ID2D1DeviceContext1 interface [Direct2D],DrawGeometryRealization method, ID2D1DeviceContext1.DrawGeometryRealization, ID2D1DeviceContext1::DrawGeometryRealization, d2d1_2/ID2D1DeviceContext1::DrawGeometryRealization, direct2d.id2d1devicecontext1_drawgeometryrealization
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d2d1_2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps \| UWP apps]
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
 - ID2D1DeviceContext1.DrawGeometryRealization
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1DeviceContext1::DrawGeometryRealization


## -description


Renders a given geometry realization to the target with the specified brush.


## -parameters




### -param geometryRealization [in]

Type: <b><a href="https://msdn.microsoft.com/EC2CF78B-5CED-494A-9ED3-407A4B6CD113">ID2D1GeometryRealization</a>*</b>

The geometry realization to be rendered.


### -param brush [in]

Type: <b><a href="https://msdn.microsoft.com/5b8f6ff8-ba52-4d30-9bea-3de89793c868">ID2D1Brush</a>*</b>

The brush to render the realization with.


## -returns



Type: <b>HRESULT</b>

The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.
            

<table>
<tr>
<th>HRESULT</th>
<th>Description</th>
</tr>
<tr>
<td>S_OK</td>
<td>No error occurred.</td>
</tr>
<tr>
<td>E_OUTOFMEMORY</td>
<td>Direct2D could not allocate sufficient memory to complete the call.
                </td>
</tr>
<tr>
<td>E_INVALIDARG</td>
<td>An invalid value was passed to the method.</td>
</tr>
</table>
 




## -remarks



This method respects all currently set state (transform, DPI, unit mode, target image, clips, layers); 
        however, artifacts such as faceting may appear when rendering the realizations with a large effective scale (either via the transform or the DPI). 
        Callers should create their realizations with an appropriate flattening tolerance using either <a href="https://msdn.microsoft.com/98a443af-4bb7-486d-bc87-ff34c3671bdd">D2D1_DEFAULT_FLATTENING_TOLERANCE</a> 
        or <a href="https://msdn.microsoft.com/62461D91-FAAF-4ABC-A852-6CD4B9B8182B">ComputeFlatteningTolerance</a> to compensate for this.
      

Additionally, callers should be aware of the safe render bounds when creating geometry realizations. 
      If a geometry extends outside of [-524,287, 524,287] DIPs in either the X- or the Y- direction in its original (pre-transform) coordinate space, 
      then it may be clipped to those bounds when it is realized. This clipping will be visible even if the realization is subsequently transformed to fit within the safe render bounds.




## -see-also




<a href="https://msdn.microsoft.com/E08FDAE4-05D3-472C-9AD9-228BAF989F1D">ID2D1DeviceContext1</a>
 

 
