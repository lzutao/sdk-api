---
UID: NF:directxmath.XMVector2Cross
title: XMVector2Cross function
author: windows-sdk-content
description: Computes the 2D cross product.
old-location: dxmath\xmvector2cross.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.geometric.XMVector2Cross(XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVector2Cross, XMVector2Cross, XMVector2Cross method [DirectX Math Support APIs], dxmath.xmvector2cross
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
 - XMVector2Cross
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVector2Cross function


## -description


Computes the 2D cross product.


## -parameters




### -param V1 [in]

2D vector.


### -param V2 [in]

2D vector.


## -returns



Returns a vector. The 2D cross product is replicated into each component.




## -remarks



The following pseudocode demonstrates the operation of the function:


```
XMVECTOR Result;

Result.x = V1.x * V2.y - v1.y * V2.x;
Result.y = V1.x * V2.y - v1.y * V2.x;
Result.z = V1.x * V2.y - v1.y * V2.x;
Result.w = V1.x * V2.y - v1.y * V2.x;

return Result;
```


Note that a 'cross-product' in 2D is not well-defined. 
    This function computes a geometric cross-product often used in 2D graphics. 
    <a href="https://msdn.microsoft.com/en-us/library/Ee420787(v=VS.85).aspx">XMVector2Orthogonal</a> is another possible interpretation of a 'cross-product' in 2D.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/a17cdad7-4fbe-bf83-472f-1b99603b7fec">DirectXMath Library 2D Vector Geometric Functions</a>
 

 
