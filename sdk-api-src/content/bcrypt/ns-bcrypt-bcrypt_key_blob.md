---
UID: NS:bcrypt._BCRYPT_KEY_BLOB
title: BCRYPT_KEY_BLOB
author: windows-sdk-content
description: Is the base structure for all CNG key BLOBs.
old-location: security\bcrypt_key_blob.htm
tech.root: seccng
ms.assetid: ae7e8db3-858d-4573-afe1-c9bc14d76480
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BCRYPT_KEY_BLOB, BCRYPT_KEY_BLOB structure [Security], bcrypt/BCRYPT_KEY_BLOB, security.bcrypt_key_blob
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: bcrypt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - BCRYPT_KEY_BLOB
product: Windows
targetos: Windows
req.typenames: BCRYPT_KEY_BLOB
req.redist: 
---

# BCRYPT_KEY_BLOB structure


## -description


The <b>BCRYPT_KEY_BLOB</b> structure is the base structure for all CNG key BLOBs. All CNG key BLOBs are based on this structure. For example, the <a href="https://msdn.microsoft.com/bbf3f4b9-5c69-4212-bb23-34bb2c84185c">BCRYPT_RSAKEY_BLOB</a> structure is based on this structure.


## -struct-fields




### -field Magic

Specifies the type of key this BLOB represents. The possible values for this member depend on the type of BLOB this structure represents.


## -see-also




<a href="https://msdn.microsoft.com/e60f6630-e4b0-4f35-a3cf-95dbcb007124">BCRYPT_ECCKEY_BLOB</a>



<a href="https://msdn.microsoft.com/bbf3f4b9-5c69-4212-bb23-34bb2c84185c">BCRYPT_RSAKEY_BLOB</a>
 

 
