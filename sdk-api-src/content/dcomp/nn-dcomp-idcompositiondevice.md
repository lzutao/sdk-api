---
UID: NN:dcomp.IDCompositionDevice
title: IDCompositionDevice
author: windows-sdk-content
description: Serves as a factory for all other Microsoft DirectComposition objects and provides methods to control transactional composition.
old-location: directcomp\idcompositiondevice.htm
tech.root: directcomp
ms.assetid: 081a14ed-c152-4e0a-b85b-1111d825ce53
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionDevice, IDCompositionDevice interface [DirectComposition], IDCompositionDevice interface [DirectComposition],described, dcomp/IDCompositionDevice, directcomp.idcompositiondevice
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
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
 - IDCompositionDevice
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionDevice interface


## -description


Serves as a factory for all other Microsoft DirectComposition objects and provides methods to control transactional composition.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDCompositionDevice</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IDCompositionDevice</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDCompositionDevice</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh707428(v=VS.85).aspx">CheckDeviceState</a>
</td>
<td align="left" width="63%">
Determines whether the DirectComposition device object is still valid.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437393(v=VS.85).aspx">Commit</a>
</td>
<td align="left" width="63%">
Commits all DirectComposition commands that are pending on this device.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437394(v=VS.85).aspx">CreateAnimation</a>
</td>
<td align="left" width="63%">
Creates an animation object that is used to animate one or more scalar properties of one or more DirectComposition objects.

  

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437395(v=VS.85).aspx">CreateEffectGroup</a>
</td>
<td align="left" width="63%">
Creates an object that represents multiple effects to be applied to a visual subtree.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437397(v=VS.85).aspx">CreateMatrixTransform</a>
</td>
<td align="left" width="63%">
Creates a 2D 3-by-2 matrix transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437398(v=VS.85).aspx">CreateMatrixTransform3D</a>
</td>
<td align="left" width="63%">
Creates a 3D 4-by-4 matrix transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437399(v=VS.85).aspx">CreateRectangleClip</a>
</td>
<td align="left" width="63%">
Creates a clip object that can be used to restrict the rendering of  a visual subtree to a rectangular area.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437400(v=VS.85).aspx">CreateRotateTransform</a>
</td>
<td align="left" width="63%">
Creates a 2D rotation transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437401(v=VS.85).aspx">CreateRotateTransform3D</a>
</td>
<td align="left" width="63%">
Creates a 3D rotation transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437402(v=VS.85).aspx">CreateScaleTransform</a>
</td>
<td align="left" width="63%">
Creates a 2D scale transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437403(v=VS.85).aspx">CreateScaleTransform3D</a>
</td>
<td align="left" width="63%">
Creates a 3D scale transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437404(v=VS.85).aspx">CreateSkewTransform</a>
</td>
<td align="left" width="63%">
Creates a 2D skew transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437405(v=VS.85).aspx">CreateSurface</a>
</td>
<td align="left" width="63%">
Creates an updateable surface object that can be associated with one or more visuals for composition.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437406(v=VS.85).aspx">CreateSurfaceFromHandle</a>
</td>
<td align="left" width="63%">
Creates a new composition surface object that wraps an existing composition surface.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437407(v=VS.85).aspx">CreateSurfaceFromHwnd</a>
</td>
<td align="left" width="63%">
Creates a wrapper object that represents the rasterization of a layered window, and that can be associated with a visual for composition.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437396(v=VS.85).aspx">CreateTargetForHwnd</a>
</td>
<td align="left" width="63%">
Creates a composition target object that is bound to the window that is represented by the specified window handle (<a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a>).

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437409(v=VS.85).aspx">CreateTransform3DGroup</a>
</td>
<td align="left" width="63%">
Creates a 3D transform group object that holds an array of 3D transform objects.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437410(v=VS.85).aspx">CreateTransformGroup</a>
</td>
<td align="left" width="63%">
Creates a 2D transform group object that holds an array of 2D transform objects.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437411(v=VS.85).aspx">CreateTranslateTransform</a>
</td>
<td align="left" width="63%">
Creates a 2D translation transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437412(v=VS.85).aspx">CreateTranslateTransform3D</a>
</td>
<td align="left" width="63%">
Creates a 3D translation transform object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437413(v=VS.85).aspx">CreateVirtualSurface</a>
</td>
<td align="left" width="63%">
Creates a sparsely populated surface that can be associated with one or more visuals for composition.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437414(v=VS.85).aspx">CreateVisual</a>
</td>
<td align="left" width="63%">
Creates a new visual object.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh437415(v=VS.85).aspx">GetFrameStatistics</a>
</td>
<td align="left" width="63%">
Retrieves information from the composition engine about composition times and the frame rate.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Hh920928(v=VS.85).aspx">WaitForCommitCompletion</a>
</td>
<td align="left" width="63%">
Waits for the composition engine to finish processing the previous call to the <a href="https://msdn.microsoft.com/en-us/library/Hh437393(v=VS.85).aspx">IDCompositionDevice::Commit</a> method. 

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh437359(v=VS.85).aspx">DCompositionCreateDevice</a>
 

 
