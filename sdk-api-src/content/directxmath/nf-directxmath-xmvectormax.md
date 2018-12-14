---
UID: NF:directxmath.XMVectorMax
title: XMVectorMax function
author: windows-sdk-content
description: Makes a per-component comparison between two vectors, and returns a vector containing the largest components.
old-location: dxmath\xmvectormax.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.arithmetic.XMVectorMax(XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorMax, XMVectorMax, XMVectorMax method [DirectX Math Support APIs], dxmath.xmvectormax
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
 - XMVectorMax
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorMax function


## -description


Makes a per-component comparison between two vectors, and returns a vector containing the largest components.


## -parameters




### -param V1 [in]

First vector to compare.


### -param V2 [in]

Second vector to compare.


## -returns



Returns a vector containing the largest components between the two vectors.




## -remarks



The following pseudocode demonstrates the operation of the function:


```
XMVECTOR Result;

Result.x = (V1.x > V2.x) ? V1.x : V2.x;
Result.y = (V1.y > V2.y) ? V1.y : V2.y;
Result.z = (V1.z > V2.z) ? V1.z : V2.z;
Result.w = (V1.w > V2.w) ? V1.w : V2.w;

return Result;
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/d7ed4516-74a6-81ec-79a2-2e39cf112d11">Vector Arithmetic Functions</a>
 

 
