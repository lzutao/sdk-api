---
UID: NS:bcrypt._BCRYPT_MULTI_OBJECT_LENGTH_STRUCT
title: BCRYPT_MULTI_OBJECT_LENGTH_STRUCT
author: windows-sdk-content
description: The BCRYPT_MULTI_OBJECT_LENGTH_STRUCT structure contains information to determine the size of the pbHashObject buffer for the BCryptCreateMultiHash function.
old-location: security\bcrypt_multi_object_length_struct.htm
tech.root: seccng
ms.assetid: CA85EA5A-4FAD-4896-BAD3-1D4C1CBD4735
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BCRYPT_MULTI_OBJECT_LENGTH_STRUCT, BCRYPT_MULTI_OBJECT_LENGTH_STRUCT structure [Security], bcrypt/BCRYPT_MULTI_OBJECT_LENGTH_STRUCT, security.bcrypt_multi_object_length_struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: bcrypt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 Update [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 Update [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Bcrypt.h
api_name:
 - BCRYPT_MULTI_OBJECT_LENGTH_STRUCT
product: Windows
targetos: Windows
req.typenames: BCRYPT_MULTI_OBJECT_LENGTH_STRUCT
req.redist: 
---

# BCRYPT_MULTI_OBJECT_LENGTH_STRUCT structure


## -description


The <b>BCRYPT_MULTI_OBJECT_LENGTH_STRUCT</b> structure contains information to determine the size of the <i>pbHashObject</i> buffer for the <a href="https://msdn.microsoft.com/en-us/library/Mt845763(v=VS.85).aspx">BCryptCreateMultiHash</a> function.


## -struct-fields




### -field cbPerObject

The number of bytes needed for the object overhead.


### -field cbPerElement

The number of bytes needed for each element of the object.


## -remarks



The size of the <i>pbHashObject</i> buffer for the <a href="https://msdn.microsoft.com/en-us/library/Mt845763(v=VS.85).aspx">BCryptCreateMultiHash</a> function is the following: <code>cbPerObject + (number of hash states) * cbPerElement</code>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Mt845763(v=VS.85).aspx">BCryptCreateMultiHash</a>
 

 
