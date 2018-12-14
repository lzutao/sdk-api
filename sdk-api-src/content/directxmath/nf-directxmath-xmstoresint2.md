---
UID: NF:directxmath.XMStoreSInt2
title: XMStoreSInt2 function
author: windows-sdk-content
description: Stores signed integer data from an XMVECTOR in an XMINT2 structure.
old-location: dxmath\xmstoresint2.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.storing.XMStoreSInt2(XMINT2@,XMVECTOR)
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Use DirectX..XMStoreSInt2, XMStoreSInt2, XMStoreSInt2 method [DirectX Math Support APIs], dxmath.xmstoresint2
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
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
 - XMStoreSInt2
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# XMStoreSInt2 function


## -description


Stores signed integer data from an <a href="https://msdn.microsoft.com/1a044094-444d-e787-fa6a-76e88531aef1">XMVECTOR</a> in an <b>XMINT2</b> structure.


## -parameters




### -param pDestination [out]

Address of an  <a href="https://msdn.microsoft.com/en-us/library/Hh404654(v=VS.85).aspx">XMINT2</a> structure in which to store the data.


### -param V

Vector containing the data to store.


## -returns



None.




## -remarks



For 16-byte aligned memory, it may be faster to use <a href="https://msdn.microsoft.com/en-us/library/Ee420362(v=VS.85).aspx">XMStoreInt2A</a> 
    with a casting operator.

The following pseudocode shows the operation of this function.


```

XMVECTOR N;	

assert(pDestination);

N = XMVectorClamp(V, MinInt, MaxInt );
N = XMVectorRound(N);

pDestination->x = (int32_t)N.v[0];
pDestination->y = (int32_t)N.v[1];

    
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/0e7b66bd-bdb0-956d-2962-b33ae52b3016">DirectXMath Library Vector Store Functions</a>
 

 
