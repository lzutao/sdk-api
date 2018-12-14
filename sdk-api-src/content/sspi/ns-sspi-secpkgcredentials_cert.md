---
UID: NS:sspi._SecPkgCredentials_Cert
title: SecPkgCredentials_Cert
author: windows-sdk-content
description: Specifies the certificate credentials. The QueryCredentialsAttributes function uses this structure.
old-location: security\secpkgcredentials_cert.htm
tech.root: secauthn
ms.assetid: 9EEE6E98-D45C-4929-9C9C-F344972D186F
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSecPkgCredentials_Cert, PSecPkgCredentials_Cert, PSecPkgCredentials_Cert structure pointer [Security], SecPkgCredentials_Cert, SecPkgCredentials_Cert structure [Security], security.secpkgcredentials_cert, sspi/PSecPkgCredentials_Cert, sspi/SecPkgCredentials_Cert"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: sspi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
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
 - SecPkgCredentials_Cert
product: Windows
targetos: Windows
req.typenames: SecPkgCredentials_Cert, *PSecPkgCredentials_Cert
req.redist: 
---

# SecPkgCredentials_Cert structure


## -description


Specifies the certificate credentials. The <a href="https://msdn.microsoft.com/a8ba6f73-8469-431b-b185-183b45b2c533">QueryCredentialsAttributes</a> function uses this structure.


## -struct-fields




### -field EncodedCertSize

Size of the encoded certificate.


### -field EncodedCert

The encoded certificate.
