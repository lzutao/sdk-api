---
UID: NF:dcomp.IDCompositionRotateTransform3D.SetAngle(float)
title: IDCompositionRotateTransform3D::SetAngle(float)
author: windows-sdk-content
description: Changes the value of the Angle property of a 3D rotation transform. The Angle property specifies the rotation angle. The default value is zero.
old-location: directcomp\idcompositionrotatetransform3d_setangle_float.htm
tech.root: directcomp
ms.assetid: A1C367E1-530C-4D4F-B93E-8C53C3DCF373
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionRotateTransform3D interface [DirectComposition],SetAngle method, IDCompositionRotateTransform3D.SetAngle, IDCompositionRotateTransform3D.SetAngle(float), IDCompositionRotateTransform3D::SetAngle, IDCompositionRotateTransform3D::SetAngle(float), SetAngle, SetAngle method [DirectComposition], SetAngle method [DirectComposition],IDCompositionRotateTransform3D interface, dcomp/IDCompositionRotateTransform3D::SetAngle, directcomp.idcompositionrotatetransform3d_setangle_float
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
 - IDCompositionRotateTransform3D.SetAngle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionRotateTransform3D::SetAngle(float)


## -description


Changes the value of the Angle property of a 3D rotation transform. The Angle property specifies the rotation angle. The default value is zero.


## -parameters




### -param angle [in]

Type: <b>float</b>

The new rotation angle, in degrees. Positive values are interpreted as the thumb-down (into the page), right hand rule where the thumb points in the Z direction and the fingers follow a clockwise direction.  Negative values are interpreted as the thumb-up (out of the page), right hand rule. For values less than -360 or greater than 360, the values wrap around and are treated as if the mathematical operation mod(360) was applied.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



This method fails if the <i>angle</i> parameter is NaN, positive infinity, or negative infinity.



If the Angle property was previously animated, this method removes the animation and sets the Angle property to the specified static value.





## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh448927(v=VS.85).aspx">IDCompositionRotateTransform3D</a>
 

 
