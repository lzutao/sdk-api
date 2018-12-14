---
UID: NS:directxpackedvector.XMDECN4
title: XMDECN4
author: windows-sdk-content
description: A 4D vector for storing signed, normalized values as 10 bit signed x-,y-, and z- components and a 2 bit signed w-component.
old-location: dxmath\xmdecn4.htm
tech.root: dxmath
ms.assetid: T:Microsoft.directx_sdk.reference.XMDECN4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMDECN4, XMDECN4 structure [DirectX Math Support APIs], directxpackedvector/XMDECN4, dxmath.xmdecn4
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: directxpackedvector.h
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
 - DirectXPackedVector.h
api_name:
 - XMDECN4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMDECN4 structure


## -description


A 4D vector for storing signed, normalized values as 10 bit signed x-,y-, and z- components
      and a 2 bit signed w-component.
  



For a list of additional functionality such as constructors and operators that are available
	using <code>XMDECN4</code> when you are programming in C++, see <a href="https://msdn.microsoft.com/en-us/library/Ee415271(v=VS.85).aspx">XMDECN4 Extensions</a>.
<div class="alert"><b>Note</b>  See <a href="https://msdn.microsoft.com/31512657-c413-9e6e-e343-1ea677a02b8c">DirectXMath Library Type
	Equivalences</a> for information about equivalent <a href="https://msdn.microsoft.com/en-us/library/Bb172533(v=VS.85).aspx">D3DDECLTYPE</a>, <a href="https://msdn.microsoft.com/en-us/library/Bb172558(v=VS.85).aspx">D3DFORMAT</a>,and <a href="https://msdn.microsoft.com/en-us/library/Bb173059(v=VS.85).aspx">DXGI_FORMAT</a> objects.
    </div><div> </div>

## -struct-fields




### -field x

Signed integer value in the range [-511, 511] describing the
			    x-coordinate of the vector.
			


### -field y

Signed integer value in the range [-511, 511] describing the
			    y-coordinate of the vector.
			


### -field z

Signed integer value in the range [-511, 511] describing the
			    z-coordinate of the vector.
			


### -field w

Signed integer value in the range [-1, 1] describing the
			    w-coordinate of the vector.
			


### -field v

Unsigned 32-bit integer representing the 4D vector.
		    


### -field XMDECN4

TBD 


### -field operator uint32_t

TBD 


### -field operator=

TBD 




## -remarks



Those <code>XMDECN4</code> constructors using floating point arguments require normalized input,
	    which must be in the range of [-1.0.-1.0]. During instantiation, the inputs
	    specifying the x-, y-, and z-components are then multiplied by 511.0f, the results are
	    rounded and then assigned to the appropriate members of <code>XMDECN4</code>.
      

<code>XMDECN4</code> can be used to load instances of <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> from
	  normalized values, by using <a href="https://msdn.microsoft.com/0c32a2a2-c3b6-4c63-ac6c-ead61df60894">XMLoadDecN4</a>, which divides the x-, y-, and
	  z-components by 511.0f, rounds the result, and then assigns the components to
	  an <code>XMVECTOR</code> instance.
      

<code>XMVECTOR</code> instances containing normalized values can be stored into <code>XMDECN4</code>using <a href="https://msdn.microsoft.com/en-us/library/Ee420317(v=VS.85).aspx">XMStoreDecN4</a>, which multiplies the x-, y-,and z-components by
	  511.0f , rounding the result, before assigning the values to the appropriate <code>XMDECN4</code>members.
      

<b>Namespace:</b> Use DirectX::PackedVector

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/58acb05d-e79b-8f42-4cf4-76ae57929739">DirectXMath Library Structures</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415271(v=VS.85).aspx">XMDECN4 Extensions</a>
 

 
