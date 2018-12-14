---
UID: NF:directxmath.XMVector3EqualR
title: XMVector3EqualR function
author: windows-sdk-content
description: Tests whether two 3D vectors are equal. In addition, this function returns a comparison value that can be examined using functions such as XMComparisonAllTrue.
old-location: dxmath\xmvector3equalr.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.comparison.XMVector3EqualR(XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVector3EqualR, XMVector3EqualR, XMVector3EqualR method [DirectX Math Support APIs], dxmath.xmvector3equalr
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
 - XMVector3EqualR
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVector3EqualR function


## -description


Tests whether two 3D vectors are equal. In addition, this function returns a comparison value that can be examined using functions such as <a href="https://msdn.microsoft.com/en-us/library/Hh437887(v=VS.85).aspx">XMComparisonAllTrue</a>.


## -parameters




### -param V1 [in]

3D vector.


### -param V2 [in]

3D vector.


## -returns



Returns a comparison value that can be examined using functions such as <a href="https://msdn.microsoft.com/en-us/library/Hh437887(v=VS.85).aspx">XMComparisonAllTrue</a>.




## -remarks



This function does the following test:


```
V1.x == V2.x
V1.y == V2.y
V1.z == V2.z
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/8c5f71fd-2ef8-86db-42de-da3da3c17e41">DirectXMath Library 3D Vector Comparison Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee420808(v=VS.85).aspx">XMVector3Equal</a>
 

 
