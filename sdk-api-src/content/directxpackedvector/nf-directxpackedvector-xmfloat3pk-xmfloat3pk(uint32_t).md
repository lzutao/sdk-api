---
UID: NF:directxpackedvector.XMFLOAT3PK.XMFLOAT3PK(uint32_t)
title: XMFLOAT3PK::XMFLOAT3PK(uint32_t)
author: windows-sdk-content
description: Initializes a new instance of XMFLOAT3PK from a uint32_tvariable containing component data in a packed format.
old-location: dxmath\xmfloat3pk_ctor_3.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMFLOAT3PK.#ctor(uint32_t)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMFLOAT3PK, XMFLOAT3PK constructor [DirectX Math Support APIs], XMFLOAT3PK constructor [DirectX Math Support APIs],XMFLOAT3PK structure, XMFLOAT3PK structure [DirectX Math Support APIs],XMFLOAT3PK constructor, XMFLOAT3PK.XMFLOAT3PK, XMFLOAT3PK.XMFLOAT3PK(uint32_t), XMFLOAT3PK::XMFLOAT3PK, XMFLOAT3PK::XMFLOAT3PK(uint32_t), dxmath.xmfloat3pk_ctor_3
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
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
req.namespace: DirectX::PackedVector
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
 - DirectXPackedVector.h
api_name:
 - XMFLOAT3PK.XMFLOAT3PK
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMFLOAT3PK::XMFLOAT3PK(uint32_t)


## -description


Initializes a new instance of <code>XMFLOAT3PK</code> from a <code>uint32_t</code>variable  containing component data in a packed format.

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/en-us/library/Ee419478(v=VS.85).aspx">XMFLOAT3PK</a> from a
  <code>uint32_t</code> variable  containing component data in a packed format.
<div class="alert"><b>Note</b>  This constructor is only available under C++.</div><div> </div>

## -parameters




### -param Packed

The values of three vector components in a packed format.
      


## -remarks



The values of the three components of the new instance of <code>XMFLOAT3PK</code> are stored
	in the argument <b>Packed</b> with the z component (as a reduced precision
	floating point number) in the most significant bits, and the x component is stored in the
	least significant bits:
 

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
  (Z10Y11X11): [32] ZZZZZzzz zzYYYYYy yyyyXXX XXxxxxxx [0]
</pre>
</td>
</tr>
</table></span></div>
Or in detail:


<ul>
<li>
Bits 0-5 of <b>v</b> are the 6 bit <i>mantissa</i> of the
	       <b>x</b> component's floating point value: the <b>xm</b> member of new instance of the structure.
	    

</li>
<li>
Bits 6-10 of <b>v</b> are the 5 bit <i>exponent</i> of the
		<b>x</b> component's floating point value the <b>xe</b> member of new instance of the structure.
	    

</li>
<li>
Bits 11-16 of <b>v</b> are the 6-bit <i>mantissa</i> of the
	       <b>y</b> component's floating point value: the <b>ym</b> member of new instance of the structure.
	    

</li>
<li>
Bits 17-21 of <b>v</b> are the 5 bit <i>exponent</i> of the
		<b>y</b> component's floating point value: the <b>ye</b> member of new instance of the structure.
	    

</li>
<li>
Bits 22-26 of <b>v</b> are the 5 bit <i>mantissa</i> of the
	       <b>z</b> component's floating point value: the <b>zm</b> member of new instance of the structure.
	    

</li>
<li>
Bits 27-31 of <b>v</b> are the 5 bit <i>exponent</i> of the
		<b>z</b> component's floating point value: the <b>ze</b> member of new instance of the structure.
	    

</li>
</ul>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Ee419478(v=VS.85).aspx">XMFLOAT3PK</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415282(v=VS.85).aspx">XMFLOAT3PK Constructors</a>
 

 
