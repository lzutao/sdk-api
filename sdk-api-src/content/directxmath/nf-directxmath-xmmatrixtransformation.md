---
UID: NF:directxmath.XMMatrixTransformation
title: XMMatrixTransformation function
author: windows-sdk-content
description: Builds a transformation matrix.
old-location: dxmath\xmmatrixtransformation.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.matrix.XMMatrixTransformation(XMVECTOR,XMVECTOR,XMVECTOR,XMVECTOR,XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMMatrixTransformation, XMMatrixTransformation, XMMatrixTransformation method [DirectX Math Support APIs], dxmath.xmmatrixtransformation
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: directxmath.h
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
req.namespace: Use DirectX.
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - DirectXMath.h
api_name:
 - XMMatrixTransformation
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMMatrixTransformation function


## -description


Builds a transformation matrix.


## -parameters




### -param ScalingOrigin [in]

3D vector describing the center of the scaling.


### -param ScalingOrientationQuaternion [in]

Quaternion describing the orientation of the scaling.


### -param Scaling [in]

3D vector containing the scaling factors for the x-axis, y-axis, and z-axis.


### -param RotationOrigin [in]

3D vector describing the center of the rotation.


### -param RotationQuaternion [in]

Quaternion describing the rotation around the origin indicated by <i>RotationOrigin</i>.


### -param Translation [in]

3D vector describing the translations along the x-axis, y-axis, and z-axis.


## -returns



Returns the transformation matrix.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/d59d0dcc-deae-3f7e-55c5-0c5ff383343b">DirectXMath Library Matrix Functions</a>
 

 
