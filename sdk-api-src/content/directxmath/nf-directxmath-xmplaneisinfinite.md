---
UID: NF:directxmath.XMPlaneIsInfinite
title: XMPlaneIsInfinite function
author: windows-sdk-content
description: Tests whether any of the coefficients of a plane is positive or negative infinity.
old-location: dxmath\xmplaneisinfinite.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.plane.XMPlaneIsInfinite(XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMPlaneIsInfinite, XMPlaneIsInfinite, XMPlaneIsInfinite method [DirectX Math Support APIs], dxmath.xmplaneisinfinite
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
 - XMPlaneIsInfinite
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMPlaneIsInfinite function


## -description


Tests whether any of the coefficients of a plane is positive or negative infinity.


## -parameters




### -param P [in]

<b>XMVECTOR</b> describing the plane coefficients (A, B, C, D) for the plane equation <code>Ax+By+Cz+D=0</code>.


## -returns



Returns true if any of the coefficients of the plane is positive or negative infinity, and false otherwise.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/6505e72e-4af5-5db3-4fc0-f83fa77692b1">DirectXMath Library Plane Functions</a>
 

 
