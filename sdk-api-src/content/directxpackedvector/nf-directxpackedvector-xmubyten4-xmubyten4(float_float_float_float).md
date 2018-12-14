---
UID: NF:directxpackedvector.XMUBYTEN4.XMUBYTEN4(float,float,float,float)
title: XMUBYTEN4::XMUBYTEN4(float,float,float,float)
author: windows-sdk-content
description: Initializes a new instance of XMUBYTEN4 from four float arguments.
old-location: dxmath\xmubyten4_ctor_4.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMUBYTEN4.#ctor(float,float,float,float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMUBYTEN4, XMUBYTEN4 constructor [DirectX Math Support APIs], XMUBYTEN4 constructor [DirectX Math Support APIs],XMUBYTEN4 structure, XMUBYTEN4 structure [DirectX Math Support APIs],XMUBYTEN4 constructor, XMUBYTEN4.XMUBYTEN4, XMUBYTEN4.XMUBYTEN4(float,float,float,float), XMUBYTEN4::XMUBYTEN4, XMUBYTEN4::XMUBYTEN4(float,float,float,float), dxmath.xmubyten4_ctor_4
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
 - XMUBYTEN4.XMUBYTEN4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMUBYTEN4::XMUBYTEN4(float,float,float,float)


## -description


Initializes a new instance of <code>XMUBYTEN4</code> from four <code>float</code> arguments.
    

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/552002c1-0000-44a6-9f43-9c958a8d1aa3">XMUBYTEN4
	</a> from four
	<code>float</code> arguments.
<div class="alert"><b>Note</b>  This constructor is only available under C++.</div><div> </div>

## -parameters




### -param _x

A normalized value for the x-coordinate of the vector.
		

This argument should be between 0.0 and 1.0. During the instantiation of an instance
		    of <code>XMUBYTEN4</code>, it is multiplied by <code>255.0f</code>, and then
		    stored as the <b>x</b> member of the structure.
		


### -param _y

A normalized value for the y-coordinate of the vector, the <b>y</b> of the new
		    instance of <code>XMUBYTEN4</code>

This argument should be between 0.0 and 1.0. During the instantiation of an
		    instance of <code>XMUBYTEN4</code>, it is multiplied by <code>255.0f</code>, and then
		    stored as the <b>y</b> member of the structure.
		


### -param _z

A normalized value for the z-coordinate of the vector, the <b>z</b> of the new
		    instance of <code>XMUBYTEN4</code>

This argument should be between 0.0 and 1.0. During the instantiation of an
		    instance of <code>XMUBYTEN4</code>, it is multiplied by <code>255.0f</code>, and then
		    stored as the <b>z</b> member of the structure.
		


### -param _w

A normalized value for the w-coordinate of the vector, the <b>w</b> of the new
		    instance of <code>XMUBYTEN4</code>

This argument should be between 0.0 and 1.0, During the instantiation of an
		    instance of <code>XMUBYTEN4</code>, it is multiplied by <code>255.0f</code>, and then
		    stored as the <b>w</b> member of the structure.
		


## -remarks



The magnitude of each argument to the constructor will be clamped to the range supported by an
	   8-bit unsigned integer [0, 255.0].
       

The following pseudocode demonstrates the operation of this constructor, which takes
	  advantage of the <code>union</code> of the four components of the <code>XMUBYTEN4</code> vector with
	  an instance of <code>uint32_t</code> in the definition of the structure:
      

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
	XMUBYTEN4 instance;
	_x1=min( max( _x, 0.0 ), 1.0 );
	_y1=min( max( _y, 0.0 ), 1.0 );
	_z1=min( max( _z, 0.0 ), 1.0 );
	_w1=min( max( _w, 0.0 ), 1.0 );
	_x = round( _x *  255.0f);
	_y = round( _y *  255.0f);
	_z = round( _z *  255.0f);
	_w = round( _w *  255.0f);
	instance.x = (uint8_t)_x1;
	instance.y = (uint8_t)_y1;
	instance.z = (uint8_t)_z1;
	instance.w = (uint8_t)_w1;
    </pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Ee420492(v=VS.85).aspx">XMUBYTEN4</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415447(v=VS.85).aspx">XMUBYTEN4 Constructors</a>
 

 
