---
UID: NF:xamlom.IVisualTreeService2.RenderTargetBitmap
title: IVisualTreeService2::RenderTargetBitmap
author: windows-sdk-content
description: Returns an image that represents the object described by handle, or returns an error if the object does not have or cannot provide such an image.
old-location: xaml_diagnostics\ivisualtreeservice2_rendertargetbitmap.htm
old-project: xaml_diagnostics
ms.assetid: BE5DA08C-46F9-44E1-89CD-85613DD3BDE4
ms.author: windowssdkdev
ms.date: 06/04/2018
ms.keywords: IVisualTreeService2 interface,RenderTargetBitmap method, IVisualTreeService2.RenderTargetBitmap, IVisualTreeService2::RenderTargetBitmap, RenderTargetBitmap, RenderTargetBitmap method, RenderTargetBitmap method,IVisualTreeService2 interface, xaml_diagnostics.ivisualtreeservice2_rendertargetbitmap, xamlom/IVisualTreeService2::RenderTargetBitmap
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: xamlom.h
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
tech.root: 
req.typenames: VisualMutationType
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - xamlom.h
api_name:
 - IVisualTreeService2.RenderTargetBitmap
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Use Windows Update or a Windows Update Services Server to retrieve the update on Windows XP.
---

# IVisualTreeService2::RenderTargetBitmap


## -description


Returns an image that represents the object described by handle, or
returns an error if the object does not have or cannot provide
such an image. 



## -parameters




### -param handle [in]

The handle associated with the visual for which the caller is requesting a bitmap.


### -param options [in]

A flag that specifies whether only the texture associated with the visual should be rendered, or whether the texture and its children should be rendered.


### -param maxPixelWidth [in]

The maximum width, in pixels, of the returned bitmap.


### -param maxPixelHeight [in]

The maximum height, in pixels, of the returned bitmap.


### -param ppBitmapData [out]

The structure containing the requested bitmap information as well as information pertaining to that bitmap.


## -returns



The possible return codes include, but are not limited to, the values shown in the following table.

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
The method succeeded. <i>ppBitmapData</i> will be set to
an <a href="https://msdn.microsoft.com/5B833E2A-D150-4ECA-88C8-CEEDBF2E23C6">IBitmapData</a> containing an image.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The image could not be acquired or converted. <i>ppBitmapData</i> will be set to
<b>NULL</b>.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
<i> handle</i> does not refer to an object that can
return an image, the <i>options</i> value is invalid, or
<i>ppBitmapData</i> is <b>NULL</b>.


</td>
</tr>
</table>
 




## -remarks



The returned image will have

<ul>
<li>Format:    <b>DXGI_FORMAT_B8G8R8A8_UNORM</b></li>
<li>AlphaMode: <b>DXGI_ALPHA_MODE_PREMULTIPLIED</b></li>
</ul>
 If the requested bitmap falls within the max pixel width and max pixel height specified, then the bitmap will be returned in its original size. If the size of the image is larger than either one of the two max values specified, then, before the bitmap is returned, the bitmap will be uniformly scaled down until its dimensions fall within the boundaries of the <i>maxPixelWidth</i> and <i>maxPixelHeight</i> specified.




## -see-also




<a href="https://msdn.microsoft.com/022E495B-2609-4CA0-A69D-BFC4A04A6F9B">IVisualTreeService2</a>
 

 
