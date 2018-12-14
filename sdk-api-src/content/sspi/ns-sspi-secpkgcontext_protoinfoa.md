---
UID: NS:sspi._SecPkgContext_ProtoInfoA
title: SecPkgContext_ProtoInfoA
author: windows-sdk-content
description: The SecPkgContext_ProtoInfo structure holds information about the protocol in use.
old-location: security\secpkgcontext_protoinfo.htm
tech.root: secauthn
ms.assetid: c10eb1fc-b957-4853-86c1-070749488bb9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSecPkgContext_ProtoInfoA, PSecPkgContext_ProtoInfo, PSecPkgContext_ProtoInfo structure pointer [Security], SecPkgContext_ProtoInfo, SecPkgContext_ProtoInfo structure [Security], SecPkgContext_ProtoInfoA, SecPkgContext_ProtoInfoW, _ssp_secpkgcontext_protoinfo, security.secpkgcontext_protoinfo, sspi/PSecPkgContext_ProtoInfo, sspi/SecPkgContext_ProtoInfo"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: sspi.h
req.include-header: Schnlsp.h
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
 - Sspi.h
api_name:
 - SecPkgContext_ProtoInfo
product: Windows
targetos: Windows
req.typenames: SecPkgContext_ProtoInfoA, *PSecPkgContext_ProtoInfoA
req.redist: 
---

# SecPkgContext_ProtoInfoA structure


## -description


<p class="CCE_Message">[The <b>SecPkgContext_ProtoInfo</b> structure is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions. Instead, use the <a href="https://msdn.microsoft.com/5380c03b-d2c5-4a0d-96a1-c39305b9c9ac">SecPkgContext_ConnectionInfo</a> structure.]

The <b>SecPkgContext_ProtoInfo</b> structure holds information about the protocol in use.

This attribute is supported only by the Schannel <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security support provider</a> (SSP).


## -struct-fields




### -field sProtocolName

Pointer to a string containing the name of the protocol.


### -field majorVersion

Major version number.


### -field minorVersion

Minor version number.
