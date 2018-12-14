---
UID: NS:directxpackedvector.XMFLOAT3SE
title: XMFLOAT3SE
author: windows-sdk-content
description: Describes a 3D vector of three floating-point components with 9 bit mantissas, each sharing the same 5-bit exponent.
old-location: dxmath\xmfloat3se.htm
tech.root: dxmath
ms.assetid: T:Microsoft.directx_sdk.reference.XMFLOAT3SE
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMFLOAT3SE, XMFLOAT3SE structure [DirectX Math Support APIs], directxpackedvector/XMFLOAT3SE, dxmath.xmfloat3se
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
 - XMFLOAT3SE
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMFLOAT3SE structure


## -description


Describes a 3D vector of three floating-point components with 9 bit mantissas, each sharing
	the same 5-bit exponent.
    

For a list of additional functionality such as constructors and operators that are available
	using <code>XMFLOAT3SE</code> when you are programming in C++, see <a href="https://msdn.microsoft.com/en-us/library/Ee415286(v=VS.85).aspx">XMFLOAT3SE Extensions</a>.


## -struct-fields




### -field xm

 


### -field ym

 


### -field zm

 


### -field e

 


### -field v

Unsigned 32-bit integer representing the 3D vector.
		    


### -field XMFLOAT3SE

TBD 


### -field operator uint32_t

TBD 


### -field operator=

TBD 




#### - e : 5

The 5-bit shared exponent.
			


#### - xm : 9

The 9-bit x component.
			


#### - ym : 9

The 9-bit y component.
			


#### - zm : 9

The 9-bit z component.
			


## -remarks



The values of the three components of an instance of <code>XMFLOAT3SE</code> are stored in
	    the <b>v</b> of the instance in the following format: the <b>e</b> member of the
	    <code>XMFLOAT3SE</code> structure -- the exponent shared by the mantissas of the
	    floating point values of all three components of <code>XMFLOAT3SE</code> -- is
	    stored in the highest order bits of the return value, and the mantissa of the x
	    component stored in the least significant bits.
	


```

   (E5Z9Y9X9): [31] EEEEEzzz zzzzzzyy yyyyyyyx xxxxxxxx [0]

```


Or in detail:
       

<ul>
<li>
Bits 0-8 of <b>Packed</b> are the 9 bit <i>mantissa</i> of the
		   <b>x</b> component's floating point value: the <b>xm</b> member of the current
		   structure.
	       

</li>
<li>
Bits 9-17 of <b>Packed</b> are the 9 bit <i>mantissa</i> of the
		   <b>y</b> component's floating point value: the <b>ym</b> member of the current
		   structure.
	       

</li>
<li>
Bits 18-26 of <b>Packed</b> are the 9 bit <i>mantissa</i> of the
		   <b>z</b> component's floating point value: the <b>zm</b> member of the current
		   structure.
	       

</li>
<li>
Bits 27-31 of <b>Packed</b> are the 5 bit <i>exponent</i> used with
		   the stored mantissas (<b>xm</b>, <b>ym</b>, <b>zm</b>) to represent the size
		   of each component: the <b>e</b> member of the current structure.
	       

</li>
</ul>
As there are no sign bits in the format for storing the components in the <code>XMFLOAT3SE</code>structure, all component values are positive.
       

<code>XMFLOAT3SE</code> can be loaded into instances of <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> by using <a href="https://msdn.microsoft.com/b0220152-6c23-4298-a974-46bdaaf0b662">XMLoadFloat3SE</a>.
       

Instances of <code>XMVECTOR</code> can be stored into an instance of <code>XMFLOAT3SE</code> with <a href="https://msdn.microsoft.com/en-us/library/Ee420338(v=VS.85).aspx">XMStoreFloat3SE</a>.
       

<b>Namespace:</b> Use DirectX::PackedVector

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/58acb05d-e79b-8f42-4cf4-76ae57929739">DirectXMath Library Structures</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415286(v=VS.85).aspx">XMFLOAT3SE Extensions</a>
 

 
