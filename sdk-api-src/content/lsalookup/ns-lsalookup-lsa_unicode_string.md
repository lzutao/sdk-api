---
UID: NS:lsalookup._LSA_UNICODE_STRING
title: LSA_UNICODE_STRING
author: windows-sdk-content
description: The LSA_UNICODE_STRING structure is used by various Local Security Authority (LSA) functions to specify a Unicode string.
old-location: security\lsa_unicode_string.htm
tech.root: secmgmt
ms.assetid: 9e1cf20f-01f9-4813-bf95-e47c5d57dcdc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PLSA_UNICODE_STRING, LSA_UNICODE_STRING, LSA_UNICODE_STRING structure [Security], PLSA_UNICODE_STRING, PLSA_UNICODE_STRING structure pointer [Security], UNICODE_STRING, _lsa_lsa_unicode_string, lsalookup/LSA_UNICODE_STRING, lsalookup/PLSA_UNICODE_STRING, security.lsa_unicode_string"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: lsalookup.h
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
 - lsalookup.h
api_name:
 - LSA_UNICODE_STRING
product: Windows
targetos: Windows
req.typenames: LSA_UNICODE_STRING, *PLSA_UNICODE_STRING
req.redist: 
---

# LSA_UNICODE_STRING structure


## -description


The <b>LSA_UNICODE_STRING</b> structure is used by various <a href="https://msdn.microsoft.com/65dd9a04-fc7c-4179-95ff-dac7dad4668f">Local Security Authority</a> (LSA) functions to specify a <a href="https://msdn.microsoft.com/264f6cb6-36c6-4cdb-b7bb-a5dbd332adcb">Unicode</a> string.


## -struct-fields




### -field Length

Specifies the length, in bytes, of the string pointed to by the <b>Buffer</b> member, not including the terminating null character, if any.


### -field MaximumLength

Specifies the total size, in bytes, of the memory allocated for <b>Buffer</b>. Up to <b>MaximumLength</b> bytes can be written into the buffer without trampling memory.


### -field Buffer

Pointer to a wide character string. Note that the strings returned by the various LSA functions might not be null-terminated.


### -field Buffer.size_is

 


### -field Buffer.size_is.MaximumLength/2

 


### -field Buffer.length_is

 


### -field Buffer.length_is.Length/2

 


