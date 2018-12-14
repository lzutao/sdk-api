---
UID: NF:directxmath.XMFLOAT4X4.XMFLOAT4X4(const float)
title: XMFLOAT4X4::XMFLOAT4X4(const float)
author: windows-sdk-content
description: Initializes a new instance of the XMFLOAT4X4 structure from a sixteen element float array.
old-location: dxmath\xmfloat4x4_ctor_3.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMFLOAT4X4.#ctor(const float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMFLOAT4X4, XMFLOAT4X4 constructor [DirectX Math Support APIs], XMFLOAT4X4 constructor [DirectX Math Support APIs],XMFLOAT4X4 structure, XMFLOAT4X4 structure [DirectX Math Support APIs],XMFLOAT4X4 constructor, XMFLOAT4X4.XMFLOAT4X4, XMFLOAT4X4.XMFLOAT4X4(const float), XMFLOAT4X4.XMFLOAT4X4(const float*), XMFLOAT4X4::XMFLOAT4X4, XMFLOAT4X4::XMFLOAT4X4(const float), dxmath.xmfloat4x4_ctor_3
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
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
 - DirectXMath.h
api_name:
 - XMFLOAT4X4.XMFLOAT4X4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMFLOAT4X4::XMFLOAT4X4(const float)


## -description


Initializes a new instance of the <code>XMFLOAT4X4</code> structure from a sixteen element
	<code>float</code> array.
    

Initializes a new instance of the <a href="https://msdn.microsoft.com/en-us/library/Ee419621(v=VS.85).aspx">XMFLOAT4X4</a> structure from a
	sixteen element <code>float</code> array.
<div class="alert"><b>Note</b>  This constructor is only available under C++.
    </div><div> </div>

## -parameters




### -param pArray

Address of a 16 element <code>float</code> array, specifying the value of each member
		of a new instance of <a href="https://msdn.microsoft.com/en-us/library/Ee419621(v=VS.85).aspx">XMFLOAT4X4</a>.
	    


## -remarks



The matrix elements are stored in <b>pArray</b> in <i>row-major</i>order.
	

The following two pseudocode examples demonstrate the operation of this constructor:
	

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
   XMFLOAT4X4 mat;
   mat._11 = pArray[0];
   mat._12 = pArray[1];
   mat._13 = pArray[2];
   mat._14 = pArray[3];
   mat._21 = pArray[4];
   mat._22 = pArray[5];
   mat._23 = pArray[6];
   mat._24 = pArray[7];
   mat._31 = pArray[8];
   mat._32 = pArray[9];
   mat._33 = pArray[10];
   mat._34 = pArray[11];
   mat._41 = pArray[12];
   mat._42 = pArray[13];
   mat._43 = pArray[14];
   mat._44 = pArray[16];
    </pre>
</td>
</tr>
</table></span></div>
Or

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
    XMFLOAT4X4 mat;
   mat.m[0,0] = pArray[0];
   mat.m[0,1] = pArray[1];
   mat.m[0,2] = pArray[2];
   mat.m[0,3] = pArray[3];
   mat.m[1,0] = pArray[4];
   mat.m[1,1] = pArray[5];
   mat.m[1,2] = pArray[6];
   mat.m[1,3] = pArray[7];
   mat.m[2,0] = pArray[8];
   mat.m[2,1] = pArray[9];
   mat.m[2,2] = pArray[10];
   mat.m[2,3] = pArray[11];
   mat.m[3,0] = pArray[12];
   mat.m[3,1] = pArray[13];
   mat.m[3,2] = pArray[14];
   mat.m[3,3] = pArray[16];
    </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Ee419621(v=VS.85).aspx">XMFLOAT4X4</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415303(v=VS.85).aspx">XMFLOAT4X4 Constructors</a>
 

 
