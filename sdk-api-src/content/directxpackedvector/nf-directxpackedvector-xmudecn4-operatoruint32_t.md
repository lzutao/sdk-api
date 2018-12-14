---
UID: NF:directxpackedvector.XMUDECN4.operator uint32_t
title: XMUDECN4::operator uint32_t
author: windows-sdk-content
description: Returns an instance of uint32_t containing the components of the XMUDECN4instance in a packed format.
old-location: dxmath\xmudecn4_operator_uint32_t.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMUDECN4.operator uint32_t
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DirectX::PackedVector.XMUDECN4.operator uint32_t, DirectX::PackedVector::XMUDECN4::operator uint32_t, XMUDECN4 structure [DirectX Math Support APIs],operator uint32_t method, XMUDECN4.operator uint32_t, XMUDECN4::operator uint32_t, dxmath.xmudecn4_operator_uint32_t, operator uint32_t, operator uint32_t method [DirectX Math Support APIs], operator uint32_t method [DirectX Math Support APIs],XMUDECN4 structure
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
 - XMUDECN4.operator uint32_t
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMUDECN4::operator uint32_t


## -description


Returns an instance of <code>uint32_t</code> containing the components of the <code>XMUDECN4</code>instance in a packed format.
    

Returns an instance of <code>uint32_t</code> containing the components of the <a href="https://msdn.microsoft.com/en-us/library/Ee420527(v=VS.85).aspx">XMUDECN4</a> instance in a packed format.
<div class="alert"><b>Note</b>  This operator is only available under C++.
    </div><div> </div>

## -parameters






## -returns



Contains the four vector components of an instance of <code>XMUDECN4</code> in a packed
		format.
	    




## -remarks



The values of the <code>XMUDECN4</code> components returned are not normalized, and are in
	    the following format:
	    
	

<ul>
<li>
The first 10 bits (bits 0- 9) of the return value are the <b>x</b>component of the current instance of <code>XMUDECN4</code>.
		

</li>
<li>
The second 10 bits (bits 10-19) of the return value are the <b>y</b>component of the current instance of <code>XMUDECN4</code>.
		

</li>
<li>
The third 10 bits (bits 20-29) of the return value are the <b>z</b>component of the current instance of <code>XMUDECN4</code>.
		

</li>
<li>
The last 2 bits (bits 30-31) of the return value are the <b>w</b> component
		    of the current instance of <code>XMUDECN4</code>.
		

</li>
</ul>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Ee420527(v=VS.85).aspx">XMUDECN4</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415455(v=VS.85).aspx">XMUDECN4 Operators</a>
 

 
