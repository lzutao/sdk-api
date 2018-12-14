---
UID: NF:directxmath.XMVectorSetIntY
title: XMVectorSetIntY function
author: windows-sdk-content
description: Set the value of the y component of an XMVECTOR Data Type.
old-location: dxmath\xmvectorsetinty.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.accessors.XMVectorSetIntY(XMVECTOR,uint32_t)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorSetIntY, XMVectorSetIntY, XMVectorSetIntY method [DirectX Math Support APIs], dxmath.xmvectorsetinty
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
 - XMVectorSetIntY
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorSetIntY function


## -description


Set the value of the <code>y</code> component of an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR Data Type</a>.


## -parameters




### -param V [in]

A valid 4D vector storing integer data.


### -param y [in]

An integer value to be assigned to <code>y</code> of <i>V</i>.


## -returns



An instance of <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR Data Type</a> whose <i>y</i> component has been set to the integer value provided by
       the argument <i>y</i> to <code>XMVectorSetIntY</code>. All other components of the returned <b>XMVECTOR Data Type</b>instance have the same value as those of the input vector <i>V</i>.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/6e7453b8-0dee-6fc5-cbac-fe20e4e3ef60">DirectXMath Library Vector Accessor Functions</a>
 

 
