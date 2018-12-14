---
UID: NF:directxmath.XMVectorSetXPtr
title: XMVectorSetXPtr function
author: windows-sdk-content
description: Sets the x component of an XMVECTOR containing floating-point data, with a value contained in an instance of float referred to by a pointer.
old-location: dxmath\xmvectorsetxptr.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.accessors.XMVectorSetXPtr(XMVECTOR,const float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVectorSetXPtr, XMVectorSetXPtr, XMVectorSetXPtr method [DirectX Math Support APIs], dxmath.xmvectorsetxptr
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
 - XMVectorSetXPtr
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVectorSetXPtr function


## -description


Sets the <code>x</code> component of an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> containing floating-point data, with a value
  contained in an instance of float referred to by a pointer.


## -parameters




### -param V

A valid 4D vector storing floating-point data.


### -param x [in]

Pointer to a float containing the value to be stored in the <code>x</code> element of the <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR Data Type</a>object <code>V</code>.


## -returns



An instance of <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR Data Type</a> whose <i>x</i> component has been set to the floating-point value
       provided by the argument <i>x</i> to <code>XMVectorSetXPtr</code>. All other components of the returned
       <b>XMVECTOR Data Type</b> instance have the same value as those of the input vector <i>V</i>.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/6e7453b8-0dee-6fc5-cbac-fe20e4e3ef60">DirectXMath Library Vector Accessor Functions</a>
 

 
