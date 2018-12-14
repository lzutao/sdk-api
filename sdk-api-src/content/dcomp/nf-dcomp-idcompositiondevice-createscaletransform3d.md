---
UID: NF:dcomp.IDCompositionDevice.CreateScaleTransform3D
title: IDCompositionDevice::CreateScaleTransform3D
author: windows-sdk-content
description: Creates a 3D scale transform object.
old-location: directcomp\idcompositiondevice_createscaletransform3d.htm
tech.root: directcomp
ms.assetid: 6B9AEEB9-559A-4B7B-A4B5-1C976B92BE7B
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateScaleTransform3D, CreateScaleTransform3D method [DirectComposition], CreateScaleTransform3D method [DirectComposition],IDCompositionDevice interface, IDCompositionDevice interface [DirectComposition],CreateScaleTransform3D method, IDCompositionDevice.CreateScaleTransform3D, IDCompositionDevice::CreateScaleTransform3D, dcomp/IDCompositionDevice::CreateScaleTransform3D, directcomp.idcompositiondevice_createscaletransform3d
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
 - IDCompositionDevice.CreateScaleTransform3D
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionDevice::CreateScaleTransform3D


## -description


Creates a 3D scale transform object.


## -parameters




### -param scaleTransform3D [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh448992(v=VS.85).aspx">IDCompositionScaleTransform3D</a>**</b>

The new 3D scale transform object. This parameter must not be NULL.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



A new 3D scale transform object has a static value of 1.0 for the ScaleX, ScaleY, and ScaleZ properties.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh437392(v=VS.85).aspx">IDCompositionDevice</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh437423(v=VS.85).aspx">IDCompositionEffectGroup::SetTransform3D</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449159(v=VS.85).aspx">IDCompositionVisual::SetEffect</a>
 

 
