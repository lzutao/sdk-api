---
UID: NF:directxmath.XMMatrixRotationNormal
title: XMMatrixRotationNormal function
author: windows-sdk-content
description: Builds a matrix that rotates around an arbitrary normal vector.
old-location: dxmath\xmmatrixrotationnormal.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.matrix.XMMatrixRotationNormal(XMVECTOR,float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMMatrixRotationNormal, XMMatrixRotationNormal, XMMatrixRotationNormal method [DirectX Math Support APIs], dxmath.xmmatrixrotationnormal
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
 - XMMatrixRotationNormal
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMMatrixRotationNormal function


## -description


Builds a matrix that rotates around an arbitrary normal vector.


## -parameters




### -param NormalAxis [in]

Normal vector describing the axis of rotation.


### -param Angle [in]

Angle of rotation in radians. Angles are measured clockwise when looking along the rotation axis toward the origin. 


## -returns



Returns the rotation matrix.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/d59d0dcc-deae-3f7e-55c5-0c5ff383343b">DirectXMath Library Matrix Functions</a>
 

 
