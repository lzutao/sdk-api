---
UID: NS:wincrypt._CMSG_HASHED_ENCODE_INFO
title: CMSG_HASHED_ENCODE_INFO
author: windows-sdk-content
description: Used with hashed messages. It is passed to the CryptMsgOpenToEncode function if the CryptMsgOpenToEncode function's dwMsgType parameter is CMSG_ENVELOPED.
old-location: security\cmsg_hashed_encode_info.htm
tech.root: seccrypto
ms.assetid: 05dfeda0-a8a1-4203-a68a-af92903ab215
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCMSG_HASHED_ENCODE_INFO, CMSG_HASHED_ENCODE_INFO, CMSG_HASHED_ENCODE_INFO structure [Security], PCMSG_HASHED_ENCODE_INFO, PCMSG_HASHED_ENCODE_INFO structure pointer [Security], _crypto2_cmsg_hashed_encode_info, security.cmsg_hashed_encode_info, wincrypt/CMSG_HASHED_ENCODE_INFO, wincrypt/PCMSG_HASHED_ENCODE_INFO"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: wincrypt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - Wincrypt.h
api_name:
 - CMSG_HASHED_ENCODE_INFO
product: Windows
targetos: Windows
req.typenames: CMSG_HASHED_ENCODE_INFO, *PCMSG_HASHED_ENCODE_INFO
req.redist: 
---

# CMSG_HASHED_ENCODE_INFO structure


## -description


The <b>CMSG_HASHED_ENCODE_INFO</b> structure is used with <a href="https://msdn.microsoft.com/4165b820-30fc-477e-a690-81109f161323">hashed</a> messages. It is passed to 
the <a href="https://msdn.microsoft.com/b0d2610b-05ba-4fb6-8f38-10f970a52091">CryptMsgOpenToEncode</a> function if the <b>CryptMsgOpenToEncode</b> function's <i>dwMsgType</i> parameter is <b>CMSG_ENVELOPED</b>.


## -struct-fields




### -field cbSize

The size, in bytes, of this structure.


### -field hCryptProv

This member is not used and should be set to <b>NULL</b>.

<b>Windows Server 2003 and Windows XP:  </b>Specifies a handle to the <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">cryptographic service provider</a> (CSP) used to do the hash. The <i>hCryptProv</i> private keys are not used. 


This member's data type is <b>HCRYPTPROV</b>.

Unless there is a strong reason for passing in a specific cryptographic provider in <i>hCryptProv</i>, pass zero to use the default RSA or DSS provider to be acquired before doing hash, signature verification, or recipient encryption operations.




### -field HashAlgorithm

A <a href="https://msdn.microsoft.com/ef0d3aa6-6b36-426f-a14c-2fdf7543deb9">CRYPT_ALGORITHM_IDENTIFIER</a> structure that contains the hash algorithm type and any associated additional parameters.


### -field pvHashAuxInfo

This member is currently not used and must be set to <b>NULL</b>.


## -see-also




<a href="https://msdn.microsoft.com/ef0d3aa6-6b36-426f-a14c-2fdf7543deb9">CRYPT_ALGORITHM_IDENTIFIER</a>
 

 
