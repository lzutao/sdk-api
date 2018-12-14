---
UID: NF:directxmath.XMVectorNotEqualInt
title: XMVectorNotEqualInt function
author: windows-sdk-content
description: Performs a per-component test for the inequality of two vectors, treating each component as an unsigned integer.
old-location: dxmath\xmvectornotequalint.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.comparison.XMVectorNotEqualInt(XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorNotEqualInt, XMVectorNotEqualInt, XMVectorNotEqualInt method [DirectX Math Support APIs], dxmath.xmvectornotequalint
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
 - XMVectorNotEqualInt
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorNotEqualInt function


## -description


Performs a per-component test for the inequality of two vectors, treating each component as an unsigned integer.


## -parameters




### -param V1 [in]

First vector to compare.


### -param V2 [in]

Second vector to compare.


## -returns



Returns a vector containing the results of each component test.




## -remarks



The following pseudocode demonstrates the operation of the function:


```
XMVECTOR Control;

Control.x = (V1.x != V2.x) ? 0xFFFFFFFF : 0;
Control.y = (V1.y != V2.y) ? 0xFFFFFFFF : 0;
Control.z = (V1.z != V2.z) ? 0xFFFFFFFF : 0;
Control.w = (V1.w != V2.w) ? 0xFFFFFFFF : 0;

return Control;

```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/c28ade14-3cf8-3d8e-260b-58751caea8d0">Bit-Wise Vector Functions</a>
 

 
