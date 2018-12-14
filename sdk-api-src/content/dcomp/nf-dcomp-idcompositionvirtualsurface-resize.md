---
UID: NF:dcomp.IDCompositionVirtualSurface.Resize
title: IDCompositionVirtualSurface::Resize
author: windows-sdk-content
description: Changes the logical size of this virtual surface object.
old-location: directcomp\idcompositionvirtualsurface_resize.htm
tech.root: directcomp
ms.assetid: BB86CDA8-1DF0-436D-9FA3-95293E2B8C0E
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionVirtualSurface interface [DirectComposition],Resize method, IDCompositionVirtualSurface.Resize, IDCompositionVirtualSurface::Resize, Resize, Resize method [DirectComposition], Resize method [DirectComposition],IDCompositionVirtualSurface interface, dcomp/IDCompositionVirtualSurface::Resize, directcomp.idcompositionvirtualsurface_resize
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
 - IDCompositionVirtualSurface.Resize
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionVirtualSurface::Resize


## -description


Changes the logical size of this virtual surface object.


## -parameters




### -param width [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The new width of the virtual surface, in pixels. The maximum width is 16,777,216 pixels.


### -param height [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The new height of the virtual surface, in pixels. The maximum height is 16,777,216 pixels.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



When a virtual surface is resized, its contents are preserved up to the new boundaries of the surface. If the surface is made smaller, any previously allocated pixels that fall outside of the new width or height are discarded.

This method fails if <a href="https://msdn.microsoft.com/en-us/library/Hh449100(v=VS.85).aspx">IDCompositionSurface::BeginDraw</a> was called for this bitmap without a corresponding call to <a href="https://msdn.microsoft.com/en-us/library/Hh449102(v=VS.85).aspx">IDCompositionSurface::EndDraw</a>.

This method fails if <i>width</i> or <i>height</i> exceeds 16,777,216 pixels. 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh437413(v=VS.85).aspx">IDCompositionDevice::CreateVirtualSurface</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449133(v=VS.85).aspx">IDCompositionVirtualSurface</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449137(v=VS.85).aspx">IDCompositionVirtualSurface::Trim</a>
 

 
