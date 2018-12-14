---
UID: NF:dcomp.IDCompositionDevice.CreateSurface
title: IDCompositionDevice::CreateSurface
author: windows-sdk-content
description: Creates an updateable surface object that can be associated with one or more visuals for composition.
old-location: directcomp\idcompositiondevice_createsurface.htm
tech.root: directcomp
ms.assetid: 3B321BF8-A7A5-4E40-B548-D88CA45F6DAF
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateSurface, CreateSurface method [DirectComposition], CreateSurface method [DirectComposition],IDCompositionDevice interface, DXGI_ALPHA_MODE_IGNORE, DXGI_ALPHA_MODE_PREMULTIPLIED, DXGI_ALPHA_MODE_UNSPECIFIED, IDCompositionDevice interface [DirectComposition],CreateSurface method, IDCompositionDevice.CreateSurface, IDCompositionDevice::CreateSurface, dcomp/IDCompositionDevice::CreateSurface, directcomp.idcompositiondevice_createsurface
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dcomp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dcomp.lib
req.dll: Dcomp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dcomp.dll
api_name:
 - IDCompositionDevice.CreateSurface
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionDevice::CreateSurface


## -description


Creates an updateable surface object that can be associated with one or more visuals for composition.


## -parameters




### -param width [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The width of the surface, in pixels.


### -param height [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The height of the surface, in pixels.


### -param pixelFormat [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a></b>

The pixel format of the surface.


### -param alphaMode [in]

Type: <b><a href="https://msdn.microsoft.com/DD3D1E49-06D2-4FB9-A41B-86453D8E566F">DXGI_ALPHA_MODE</a></b>

The format of the alpha channel, if an alpha channel is included in the pixel format. It can be one of the following values:

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="DXGI_ALPHA_MODE_UNSPECIFIED"></a><a id="dxgi_alpha_mode_unspecified"></a><dl>
<dt><b>DXGI_ALPHA_MODE_UNSPECIFIED</b></dt>
</dl>
</td>
<td width="60%">
The alpha channel is not specified. This value has the same effect as <b>DXGI_ALPHA_MODE_IGNORE</b>.

</td>
</tr>
<tr>
<td width="40%"><a id="DXGI_ALPHA_MODE_PREMULTIPLIED"></a><a id="dxgi_alpha_mode_premultiplied"></a><dl>
<dt><b>DXGI_ALPHA_MODE_PREMULTIPLIED</b></dt>
</dl>
</td>
<td width="60%">
The color channels contain values that are premultiplied with the alpha channel.


</td>
</tr>
<tr>
<td width="40%"><a id="DXGI_ALPHA_MODE_IGNORE"></a><a id="dxgi_alpha_mode_ignore"></a><dl>
<dt><b>DXGI_ALPHA_MODE_IGNORE</b></dt>
</dl>
</td>
<td width="60%">
The alpha channel should be ignored and the bitmap should be rendered opaquely.

</td>
</tr>
</table>
 


### -param surface [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh449083(v=VS.85).aspx">IDCompositionSurface</a>**</b>

The newly created surface object. This parameter must not be NULL.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



A Microsoft DirectComposition surface is a rectangular array of pixels that can be associated with a visual for composition. 

A newly created surface object is in an uninitialized state. While it is uninitialized, the surface has no effect on the composition of the visual tree. It behaves exactly like a surface that has  100% transparent pixels.



To initialize the surface with pixel data, use the <b>IDCompositionSurface::BeginDraw</b> method. The first call to this method must cover the entire surface area to provide an initial value for every pixel. Subsequent calls may specify smaller sub-rectangles of the surface to update.



DirectComposition surfaces support the following pixel formats: 

<ul>
<li><b>DXGI_FORMAT_B8G8R8A8_UNORM</b></li>
<li><b>DXGI_FORMAT_R8G8B8A8_UNORM</b></li>
<li><b>DXGI_FORMAT_R16G16B16A16_FLOAT</b></li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh437392(v=VS.85).aspx">IDCompositionDevice</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh437413(v=VS.85).aspx">IDCompositionDevice::CreateVirtualSurface</a>
 

 
