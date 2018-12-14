---
UID: NF:directxpackedvector.XMFLOAT3PK.operator uint32_t
title: XMFLOAT3PK::operator uint32_t
author: windows-sdk-content
description: Returns an instance of uint32_t containing the components of the XMFLOAT3PK instance in a packed format.
old-location: dxmath\xmfloat3pk_operator_uint32_t.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMFLOAT3PK.operator uint32_t
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DirectX::PackedVector.XMFLOAT3PK.operator uint32_t, DirectX::PackedVector::XMFLOAT3PK::operator uint32_t, XMFLOAT3PK structure [DirectX Math Support APIs],operator uint32_t method, XMFLOAT3PK.operator uint32_t, XMFLOAT3PK::operator uint32_t, dxmath.xmfloat3pk_operator_uint32_t, operator uint32_t, operator uint32_t method [DirectX Math Support APIs], operator uint32_t method [DirectX Math Support APIs],XMFLOAT3PK structure
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
 - XMFLOAT3PK.operator uint32_t
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMFLOAT3PK::operator uint32_t


## -description


Returns an instance of <code>uint32_t</code> containing the components of the
<code>XMFLOAT3PK</code> instance in a packed format.

This operator returns an instance of <code>uint32_t</code> containing the components of the
    <a href="https://msdn.microsoft.com/en-us/library/Ee419478(v=VS.85).aspx">XMFLOAT3PK</a> instance in a packed format.

<div class="alert"><b>Note</b>  This operator is only available under C++.</div><div> </div>

## -parameters






## -returns



Contains the three vector components of an instance of
	  <code>XMFLOAT3PK</code> in a packed format.
      




## -remarks



The values of the three components of the current instance of <code>XMFLOAT3PK</code> are
	returned packed in a <code>uint32_t</code> with the z component (as a reduced precision floating
	point number) in the most significant bits, and the x component is stored in the least
	significant bits:
 

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
  (Z10Y11X11): [32] ZZZZZzzz zzYYYYYY yyyyyXXX XXXxxxxx [0]
</pre>
</td>
</tr>
</table></span></div>
Or in detail:


<ul>
<li>
Bits 0-5 of the return value are the 6 bit <i>mantissa</i> of the
	       <b>x</b> component's floating point value.
	    

</li>
<li>
Bits 6-10 of the return value are the 5 bit <i>exponent</i> of the
		<b>x</b> component's floating point value.
	    

</li>
<li>
Bits 11-16 of the return value are the 6-bit <i>mantissa</i> of the
	       <b>y</b> component's floating point value.
	    

</li>
<li>
Bits 17-21 of the return value are the 5 bit <i>exponent</i> of the
		<b>y</b> component's floating point value.
	    

</li>
<li>
Bits 22-26 of the return value are the 5 bit <i>mantissa</i> of the
	       <b>z</b> component's floating point value.
	    

</li>
<li>
Bits 27-31 of the return value are the 5 bit <i>exponent</i> of the
		<b>z</b> component's floating point value.
	    

</li>
</ul>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Ee419478(v=VS.85).aspx">XMFLOAT3PK</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415284(v=VS.85).aspx">XMFLOAT3PK Operators</a>
 

 
