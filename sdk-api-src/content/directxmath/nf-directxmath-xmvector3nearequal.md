---
UID: NF:directxmath.XMVector3NearEqual
title: XMVector3NearEqual function
author: windows-sdk-content
description: Tests whether one 3D vector is near another 3D vector.
old-location: dxmath\xmvector3nearequal.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.comparison.XMVector3NearEqual(XMVECTOR,XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVector3NearEqual, XMVector3NearEqual, XMVector3NearEqual method [DirectX Math Support APIs], dxmath.xmvector3nearequal
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
 - XMVector3NearEqual
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVector3NearEqual function


## -description


Tests whether one 3D vector is near another 3D vector.


## -parameters




### -param V1 [in]

3D vector.


### -param V2 [in]

3D vector.


### -param Epsilon [in]

Tolerance value used for judging equality.


## -returns



Returns true if <i>V1</i> is near <i>V2</i> and false otherwise. 




## -remarks



The following pseudocode demonstrates the operation of the function:


```
return ( ( abs( V1.x - V2.x ) <= Epsilon ) && 
         ( abs( V1.y - V2.y ) <= Epsilon ) && 
         ( abs( V1.z - V2.z ) <= Epsilon ));
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/8c5f71fd-2ef8-86db-42de-da3da3c17e41">DirectXMath Library 3D Vector Comparison Functions</a>
 

 
