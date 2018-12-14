---
UID: NF:directxmath.XMQuaternionBaryCentricV
title: XMQuaternionBaryCentricV function
author: windows-sdk-content
description: Returns a point in barycentric coordinates, using the specified quaternions.
old-location: dxmath\xmquaternionbarycentricv.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.quaternion.XMQuaternionBaryCentricV(XMVECTOR,XMVECTOR,XMVECTOR,XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMQuaternionBaryCentricV, XMQuaternionBaryCentricV, XMQuaternionBaryCentricV method [DirectX Math Support APIs], dxmath.xmquaternionbarycentricv
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
 - XMQuaternionBaryCentricV
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMQuaternionBaryCentricV function


## -description


Returns a point in barycentric coordinates, using the specified quaternions.


## -parameters




### -param Q0 [in]

First quaternion in the triangle.


### -param Q1 [in]

Second quaternion in the triangle.


### -param Q2 [in]

Third quaternion in the triangle.


### -param F [in]

Weighting factor. All components of this vector must be the same.


### -param G [in]

Weighting factor. All components of this vector must be the same.


## -returns



Returns a quaternion in barycentric coordinates.




## -remarks



The DirectXMath quaternion functions use an XMVECTOR 4-vector to represent quaternions, 
    where the X, Y, and Z components are the vector part and the W component is the scalar part.

This function is identical to <a href="https://msdn.microsoft.com/a312a8c9-7e50-4a80-819f-efe232074513">XMQuaternionBaryCentric</a> except
   that <i>F</i> and <i>G</i> are supplied using a 4D vector instead of a <b>float</b> value.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/2d397c98-d0cd-08e0-6104-cca31bb6bd11">DirectXMath Library Quaternion Functions</a>



<a href="https://msdn.microsoft.com/a312a8c9-7e50-4a80-819f-efe232074513">XMQuaternionBaryCentric</a>
 

 
