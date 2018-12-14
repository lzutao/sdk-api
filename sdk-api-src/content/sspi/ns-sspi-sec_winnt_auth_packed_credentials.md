---
UID: NS:sspi._SEC_WINNT_AUTH_PACKED_CREDENTIALS
title: SEC_WINNT_AUTH_PACKED_CREDENTIALS
author: windows-sdk-content
description: Specifies serialized credentials.
old-location: security\sec_winnt_auth_packed_credentials.htm
tech.root: secauthn
ms.assetid: 9a21f0cd-d4e1-4aa8-8d0d-72bc7002ce32
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSEC_WINNT_AUTH_PACKED_CREDENTIALS, PSEC_WINNT_AUTH_PACKED_CREDENTIALS, PSEC_WINNT_AUTH_PACKED_CREDENTIALS structure pointer [Security], SEC_WINNT_AUTH_PACKED_CREDENTIALS, SEC_WINNT_AUTH_PACKED_CREDENTIALS structure [Security], security.sec_winnt_auth_packed_credentials, sspi/PSEC_WINNT_AUTH_PACKED_CREDENTIALS, sspi/SEC_WINNT_AUTH_PACKED_CREDENTIALS"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: sspi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - Sspi.h
api_name:
 - SEC_WINNT_AUTH_PACKED_CREDENTIALS
product: Windows
targetos: Windows
req.typenames: SEC_WINNT_AUTH_PACKED_CREDENTIALS, *PSEC_WINNT_AUTH_PACKED_CREDENTIALS
req.redist: 
---

# SEC_WINNT_AUTH_PACKED_CREDENTIALS structure


## -description


Specifies serialized credentials.


## -struct-fields




### -field cbHeaderLength

The size, in bytes, of the structure header.


### -field cbStructureLength

The size, in bytes, of this structure.


### -field AuthData

Specifies the type of the credential, and the offset and size of the serialized data.
