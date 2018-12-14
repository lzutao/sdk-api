---
UID: NF:dcomp.IDCompositionScaleTransform3D.SetScaleY
title: IDCompositionScaleTransform3D::SetScaleY
author: windows-sdk-content
description: Changes the value of the ScaleY property of a 3D scale transform.
old-location: directcomp\idcompositionscaletransform3d_setscaley_float.htm
tech.root: directcomp
ms.assetid: F4BC7859-DD50-4AD0-8B6C-4E353B0AE334
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionScaleTransform3D interface [DirectComposition],SetScaleY method, IDCompositionScaleTransform3D.SetScaleY, IDCompositionScaleTransform3D::SetScaleY, IDCompositionScaleTransform3D::SetScaleY(float), SetScaleY, SetScaleY method [DirectComposition], SetScaleY method [DirectComposition],IDCompositionScaleTransform3D interface, dcomp/IDCompositionScaleTransform3D::SetScaleY, directcomp.idcompositionscaletransform3d_setscaley_float
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
 - IDCompositionScaleTransform3D.SetScaleY
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionScaleTransform3D::SetScaleY


## -description


Changes the value of the ScaleY property of a 3D scale transform. The ScaleY property specifies the scale factor along the y-axis.


## -parameters




### -param scaleY [in]

Type: <b>float</b>

The new y-axis scale factor.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



This method fails if the <i>scaleY</i> parameter is NaN, positive infinity, or negative infinity.



If the ScaleY property was previously animated, this method removes the animation and sets the ScaleY property to the specified static value.





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh448990(v=VS.85).aspx">IDCompositionScaleTransform3D</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449018(v=VS.85).aspx">IDCompositionScaleTransform3D::SetScaleX</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449030(v=VS.85).aspx">IDCompositionScaleTransform3D::SetScaleZ</a>
 

 
