---
UID: NF:directxpackedvector.XMCOLOR.operator uint32_t
title: XMCOLOR::operator uint32_t
author: windows-sdk-content
description: Returns an instance of uint32_t containing the components of the XMCOLORinstance in a packed format.
old-location: dxmath\xmcolor_operator_uint32_t.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMCOLOR.operator uint32_t
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DirectX::PackedVector.XMCOLOR.operator uint32_t, DirectX::PackedVector::XMCOLOR::operator uint32_t, XMCOLOR structure [DirectX Math Support APIs],operator uint32_t method, XMCOLOR.operator uint32_t, XMCOLOR::operator uint32_t, dxmath.xmcolor_operator_uint32_t, operator uint32_t, operator uint32_t method [DirectX Math Support APIs], operator uint32_t method [DirectX Math Support APIs],XMCOLOR structure
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
 - XMCOLOR.operator uint32_t
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMCOLOR::operator uint32_t


## -description


Returns an instance of <code>uint32_t</code> containing the components of the <code>XMCOLOR</code>instance in a packed format.
<div class="alert"><b>Note</b>  This operator is only available under C++.
    </div><div> </div>

## -parameters






## -returns



Contains the four color channel value components of an instance of
		<code>XMCOLOR</code> in a packed format.
	    




## -remarks



The values of the <code>XMCOLOR</code> color channels components returned are not
	    normalized, and are in the following format:
	    
	

<ul>
<li>
The first 8 bits (bits 0-7) of the return value are the <b>a</b> member (alpha
		    channel) of the current instance of <code>XMCOLOR</code>.
		

</li>
<li>
The second 8 bits (bits 8-15) of the return value are the <b>r</b> member (red
		    color channel) of the current instance of <code>XMCOLOR</code>.
		

</li>
<li>
The third 8 bits (bits 16-23) of the return value are the <b>g</b> member (green
		    color channel) of the current instance of <code>XMCOLOR</code>.
		

</li>
<li>
The fourth 8 bits (bits 24-31) of the return value are the <b>b</b> member (blue
		    color channel) of the current instance of <code>XMCOLOR</code>.
		

</li>
</ul>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Ee419292(v=VS.85).aspx">XMCOLOR</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415266(v=VS.85).aspx">XMCOLOR Operators</a>
 

 
