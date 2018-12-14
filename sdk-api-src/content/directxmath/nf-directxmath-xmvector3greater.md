---
UID: NF:directxmath.XMVector3Greater
title: XMVector3Greater function
author: windows-sdk-content
description: Tests whether one 3D vector is greater than another 3D vector.
old-location: dxmath\xmvector3greater.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.comparison.XMVector3Greater(XMVECTOR,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVector3Greater, XMVector3Greater, XMVector3Greater method [DirectX Math Support APIs], dxmath.xmvector3greater
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
 - XMVector3Greater
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVector3Greater function


## -description


Tests whether one 3D vector is greater than another 3D vector.


## -parameters




### -param V1 [in]

3D vector.


### -param V2 [in]

3D vector.


## -returns



Returns true if <i>V1</i> is greater than <i>V2</i> and false otherwise. See the remarks section.




## -remarks



The following pseudocode demonstrates the operation of the function:


```
return ( V1.x > V2.x && V1.y > V2.y &&
         V1.z > V2.z );
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/8c5f71fd-2ef8-86db-42de-da3da3c17e41">DirectXMath Library 3D Vector Comparison Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee420815(v=VS.85).aspx">XMVector3GreaterR</a>
 

 
