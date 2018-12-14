---
UID: NF:directxpackedvector.XMFLOAT3SE.XMFLOAT3SE(float,float,float)
title: XMFLOAT3SE::XMFLOAT3SE(float,float,float)
author: windows-sdk-content
description: Initializes a new instance of XMFLOAT3SE from three float arguments.
old-location: dxmath\xmfloat3se_ctor_2.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.reference.XMFLOAT3SE.#ctor(float,float,float)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: XMFLOAT3SE, XMFLOAT3SE constructor [DirectX Math Support APIs], XMFLOAT3SE constructor [DirectX Math Support APIs],XMFLOAT3SE structure, XMFLOAT3SE structure [DirectX Math Support APIs],XMFLOAT3SE constructor, XMFLOAT3SE.XMFLOAT3SE, XMFLOAT3SE.XMFLOAT3SE(float,float,float), XMFLOAT3SE::XMFLOAT3SE, XMFLOAT3SE::XMFLOAT3SE(float,float,float), dxmath.xmfloat3se_ctor_2
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
 - XMFLOAT3SE.XMFLOAT3SE
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMFLOAT3SE::XMFLOAT3SE(float,float,float)


## -description


Initializes a new instance of <code>XMFLOAT3SE</code> from three <code>float</code> arguments.

This constructor initializes a new instance of <a href="https://msdn.microsoft.com/en-us/library/Ee419489(v=VS.85).aspx">XMFLOAT3SE</a> from three
  <code>float</code> arguments.
<div class="alert"><b>Note</b>  This constructor is only available under C++.</div><div> </div>

## -parameters




### -param _x

Value to be stored in the x-component of the new instance of <code>XMFLOAT3SE</code>.
	  

The value stored is transformed from the standard 32 floating point format (sign bit,
	      8 bit exponent, 23 bit mantissa), to an 14 bit floating point format (9 bit mantissa,
	      and 5 bit exponent).  
	  


### -param _y

Value to be stored in the y-component of the new instance of <code>XMFLOAT3SE</code>.
	  

The value stored is transformed from the standard 32 floating point format (sign bit,
	      8 bit exponent, 23 bit mantissa), to an 14 bit floating point format (9 bit mantissa,
	      and 5 bit exponent).  
	  


### -param _z

Value to be stored in the z-component of the new instance of <code>XMFLOAT3SE</code>.
	  

The value stored is transformed from the standard 32 floating point format (sign bit,
	      8 bit exponent, 23 bit mantissa), to an 14 bit floating point format (9 bit mantissa,
	      and 5 bit exponent).  
	  


## -remarks



As the floating point storage formats used by <code>XMFLOAT3SE</code> do not support a sign
	   bit, all arguments to this constructor must be greater than or equal to zero.
       

The floating point values of all components are all expressed using the same exponent,
	   which is stored in the <b>e</b> member of the new instance of <code>XMFLOAT3SE</code>instantiated by this constructor.
       

Because of the change in floating point format during the instantiation of an instance of
	   <code>XMFLOAT3SE</code>, some loss of precision can be expected.
       




## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Ee419489(v=VS.85).aspx">XMFLOAT3SE</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee415285(v=VS.85).aspx">XMFLOAT3SE Constructors</a>
 

 
