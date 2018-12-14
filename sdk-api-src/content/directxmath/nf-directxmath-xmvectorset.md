---
UID: NF:directxmath.XMVectorSet
title: XMVectorSet function
author: windows-sdk-content
description: Creates a vector using four floating-point values.
old-location: dxmath\xmvectorset.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.initialization.XMVectorSet(float,float,float,float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorSet, XMVectorSet, XMVectorSet method [DirectX Math Support APIs], dxmath.xmvectorset
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
 - XMVectorSet
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorSet function


## -description


Creates a vector using four floating-point values.


## -parameters




### -param x [in]

The x component of the vector to return.


### -param y [in]

The y component of the vector to return.


### -param z [in]

The z component of the vector to return.


### -param w [in]

The w component of the vector to return.


## -returns



An instance <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> each of whose four components
(<i>x</i>,<i>y</i>,<i>z</i>, and <i>w</i>) is a
floating-point number with the same value as the corresponding input argument to
<code>XMVectorSet</code>.




## -remarks



The following pseudocode demonstrates the operation of the function:


```
XMVECTOR V;
float x,y,z,w;
V.x = x;
V.y = y;
V.z = z;
V.w = w;

return V;
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/862a1a83-2371-9885-20d4-184aae52fd10">Vector Initialization Functions</a>
 

 
