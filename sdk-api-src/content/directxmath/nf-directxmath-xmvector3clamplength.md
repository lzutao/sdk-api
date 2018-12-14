---
UID: NF:directxmath.XMVector3ClampLength
title: XMVector3ClampLength function
author: windows-sdk-content
description: Clamps the length of a 3D vector to a given range.
old-location: dxmath\xmvector3clamplength.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.geometric.XMVector3ClampLength(XMVECTOR,float,float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVector3ClampLength, XMVector3ClampLength, XMVector3ClampLength method [DirectX Math Support APIs], dxmath.xmvector3clamplength
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: directxmath.h
req.include-header: DirectXMath.h
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
 - directxmathvector.inl
api_name:
 - XMVector3ClampLength
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVector3ClampLength function


## -description


Clamps the length of a 3D vector to a given range.


## -parameters




### -param V [in]

3D vector.


### -param LengthMin [in]

Minimum clamp length.


### -param LengthMax [in]

Maximum clamp length.


## -returns



Returns a 3D vector whose length is clamped to the specified minimum and maximum.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/f2cee697-b4ec-5e4d-a87b-622c9fb7997c">DirectXMath Library 3D Vector Geometric Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee420804(v=VS.85).aspx">XMVector3ClampLengthV</a>
 

 
