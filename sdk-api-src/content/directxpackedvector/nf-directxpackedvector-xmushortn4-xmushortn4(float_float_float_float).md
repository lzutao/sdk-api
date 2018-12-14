---
UID: NF:directxpackedvector.XMUSHORTN4.XMUSHORTN4(float,float,float,float)
title: XMUSHORTN4::XMUSHORTN4(float,float,float,float)
author: windows-sdk-content
description: Initializes a new instance of XMUSHORTN4 from four normalized floatarguments.
old-location: dxmath\xmushortn4_ctor_4.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMUSHORTN4.#ctor(float,float,float,float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMUSHORTN4, XMUSHORTN4 constructor [DirectX Math Support APIs], XMUSHORTN4 constructor [DirectX Math Support APIs],XMUSHORTN4 structure, XMUSHORTN4 structure [DirectX Math Support APIs],XMUSHORTN4 constructor, XMUSHORTN4.XMUSHORTN4, XMUSHORTN4.XMUSHORTN4(float,float,float,float), XMUSHORTN4::XMUSHORTN4, XMUSHORTN4::XMUSHORTN4(float,float,float,float), dxmath.xmushortn4_ctor_4
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
 - XMUSHORTN4.XMUSHORTN4
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMUSHORTN4::XMUSHORTN4(float,float,float,float)


## -description


Initializes a new instance of <code>XMUSHORTN4</code> from four normalized <code>float</code>arguments.
    

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/en-us/library/Ee420726(v=VS.85).aspx">XMUSHORTN4</a> from four
	normalized <code>float</code> arguments.
<div class="alert"><b>Note</b>  This constructor is only available under C++.</div><div> </div>

## -parameters




### -param _x

A normalized value for the x-coordinate of the vector.
		

This argument should be between 0.0 and 1.0; during the instantiation of
		    an instance of <code>XMUSHORTN4</code>, it is multiplied by <code>65535.0f</code> and
		    then stored as the <b>x</b> member of the structure.
		


### -param _y

A normalized value for the y-coordinate of the vector, the <b>y</b> of the
		    new instance of <code>XMUSHORTN4</code>.
		

This argument should be between 0.0 and 1.0; during the instantiation of
		    an instance of <code>XMUSHORTN4</code>, it is multiplied by <code>65535.0f</code> and
		    then stored as the <b>y</b> member of the structure.
		


### -param _z

A normalized value for the z-coordinate of the vector, the <b>z</b> of the
		    new instance of <code>XMUSHORTN4</code>.
		

This argument should be between 0.0 and 1.0; during the instantiation of
		    an instance of <code>XMUSHORTN4</code>, it is multiplied by <code>65535.0f</code> and
		    then stored as the <b>z</b> member of the structure.
		


### -param _w

A normalized value for the w-coordinate of the vector, the <b>w</b> of the
		    new instance of <code>XMUSHORTN4</code>.
		

This argument should be between 0.0 and 1.0; during the instantiation of
		    an instance of <code>XMUSHORTN4</code>, it is multiplied by <code>65535.0f</code> and
		    then stored as the <b>w</b> member of the structure.
		


## -remarks



All input values,<i>_x</i>,<i>_y</i>, <i>_z</i>, and <i>_w</i> are
	    clamped to a range of -1.0 to 1.0.
	

The following pseudocode demonstrates the operation of this constructor:
	

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>
	XMUSHORTN4 instance;
	_x1=min( max( _x, 0.0 ), 1.0 );
	_y1=min( max( _y, 0.0 ), 1.0 );
	_z1=min( max( _z, 0.0 ), 1.0 );
	_w1=min( max( _w, 0.0 ), 1.0 );
	_x1 = round( _x1 * 65535.0f);
	_y1 = round( _y1 * 65535.0f);
	_z1 = round( _z1 * 65535.0f);
	_w1 = round( _w1 * 65535.0f);
	instance._x = _x1;
	instance._y = _y1;
	instance._z = _z1;
	instance._w = _w1;
	</pre>
</td>
</tr>
</table></span></div>



## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Ee420726(v=VS.85).aspx">XMUSHORTN4</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415513(v=VS.85).aspx">XMUSHORTN4 Constructors</a>
 

 
