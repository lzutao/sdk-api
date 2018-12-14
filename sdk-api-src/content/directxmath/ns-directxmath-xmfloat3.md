---
UID: NS:directxmath.XMFLOAT3
title: XMFLOAT3
author: windows-sdk-content
description: Describes a 3D vector consisting of three single-precision floating-point values.
old-location: dxmath\xmfloat3.htm
tech.root: dxmath
ms.assetid: T:Microsoft.directx_sdk.reference.XMFLOAT3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMFLOAT3, XMFLOAT3 structure [DirectX Math Support APIs], directxmath/XMFLOAT3, dxmath.xmfloat3
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: directxmath.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - DirectXMath.h
api_name:
 - XMFLOAT3
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMFLOAT3 structure


## -description


Describes a 3D vector consisting of three single-precision floating-point values.

For a list of additional functionality such as constructors and operators that are available using <code>XMFLOAT3</code> when you
  are programming in C++, see <a href="https://msdn.microsoft.com/en-us/library/Ee415293(v=VS.85).aspx">XMFLOAT3 Extensions</a>.
<div class="alert"><b>Note</b>  See <a href="https://msdn.microsoft.com/31512657-c413-9e6e-e343-1ea677a02b8c">DirectXMath Library Type Equivalences</a> for information
  about equivalent <a href="https://msdn.microsoft.com/en-us/library/Bb172533(v=VS.85).aspx">D3DDECLTYPE</a>, <a href="https://msdn.microsoft.com/en-us/library/Bb172558(v=VS.85).aspx">D3DFORMAT</a>, and
  <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a> objects.</div><div> </div>

## -struct-fields




### -field x

<b>float</b> value describing the x-coordinate of the vector.


### -field y

<b>float</b> value describing the y-coordinate of the vector.


### -field z

<b>float</b> value describing the z-coordinate of the vector.


### -field operator=

TBD 


### -field XMFLOAT3

TBD 




## -remarks



<code>XMFLOAT3</code> can be loaded into instances of <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1"> XMVECTOR</a> by using
   <a href="https://msdn.microsoft.com/4564cbae-f99b-46dc-91ba-93b8018d17bb">XMLoadFloat3</a>.

Instances of <code>XMVECTOR</code> can be stored into an instance of <code>XMFLOAT3</code> with
   <a href="https://msdn.microsoft.com/en-us/library/Ee420329(v=VS.85).aspx">XMStoreFloat3</a>.

<b>Namespace:</b> Use DirectX

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/58acb05d-e79b-8f42-4cf4-76ae57929739">DirectXMath Library Structures</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415293(v=VS.85).aspx">XMFLOAT3 Extensions</a>
 

 
