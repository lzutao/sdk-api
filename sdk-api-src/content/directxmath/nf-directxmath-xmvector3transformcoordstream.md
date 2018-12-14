---
UID: NF:directxmath.XMVector3TransformCoordStream
title: XMVector3TransformCoordStream function
author: windows-sdk-content
description: Transforms a stream of 3D vectors by a given matrix, projecting the resulting vectors such that their w coordinates are equal to 1.0.
old-location: dxmath\xmvector3transformcoordstream.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.transformation.XMVector3TransformCoordStream(XMFLOAT3@,size_t,const XMFLOAT3,size_t,size_t,XMMATRIX)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMVector3TransformCoordStream, XMVector3TransformCoordStream, XMVector3TransformCoordStream method [DirectX Math Support APIs], dxmath.xmvector3transformcoordstream
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: directxmath.h
req.include-header: DirectXMath.h
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
 - directxmathvector.inl
api_name:
 - XMVector3TransformCoordStream
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMVector3TransformCoordStream function


## -description


Transforms a stream of 3D vectors by a given matrix, projecting the resulting vectors such that their w coordinates are
  equal to 1.0.


## -parameters




### -param pOutputStream [out]

Address of the first <a href="https://msdn.microsoft.com/en-us/library/Ee419475(v=VS.85).aspx">XMFLOAT3</a> in the destination stream.


### -param OutputStride [in]

Stride, in bytes, between vectors in the destination stream.


### -param pInputStream [in]

Address of the first <a href="https://msdn.microsoft.com/en-us/library/Ee419475(v=VS.85).aspx">XMFLOAT3</a> in the stream to be transformed.


### -param InputStride [in]

Stride, in bytes, between vectors in the input stream.


### -param VectorCount [in]

Number of vectors to transform.


### -param M [in]

Transformation matrix.


## -returns



Returns the address of the first <a href="https://msdn.microsoft.com/en-us/library/Ee419475(v=VS.85).aspx">XMFLOAT3</a> in the destination stream.




## -remarks



<code>XMVector3TransformCoordStream</code> ignores the w component of the input vector, and uses a value of 1.0 instead. The w component of the returned vectors will always be 1.0.

<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/148972da-e460-63b9-6b01-10201f63d157">DirectXMath Library 3D Vector Transformation Functions</a>



<a href="https://msdn.microsoft.com/en-us/library/Ee420943(v=VS.85).aspx">XMVector3TransformCoord</a>
 

 
