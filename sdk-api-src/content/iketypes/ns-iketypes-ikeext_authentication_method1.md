---
UID: NS:iketypes.IKEEXT_AUTHENTICATION_METHOD1_
title: IKEEXT_AUTHENTICATION_METHOD1
author: windows-sdk-content
description: Specifies various parameters for IKE/Authip authentication.
old-location: fwp\ikeext_authentication_method1.htm
tech.root: fwp
ms.assetid: 55894ac3-2cb7-4828-8346-9ca66ce3253a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IKEEXT_AUTHENTICATION_METHOD1, IKEEXT_AUTHENTICATION_METHOD1 structure [Filtering], fwp.ikeext_authentication_method1, iketypes/IKEEXT_AUTHENTICATION_METHOD1
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: iketypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Iketypes.idl
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
 - Iketypes.h
api_name:
 - IKEEXT_AUTHENTICATION_METHOD1
product: Windows
targetos: Windows
req.typenames: IKEEXT_AUTHENTICATION_METHOD1
req.redist: 
---

# IKEEXT_AUTHENTICATION_METHOD1 structure


## -description


The <b>IKEEXT_AUTHENTICATION_METHOD1</b> structure specifies various parameters for IKE/Authip authentication.<div class="alert"><b>Note</b>  <b>IKEEXT_AUTHENTICATION_METHOD1</b> is the specific implementation of IKEEXT_AUTHENTICATION_METHOD used in Windows 7. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows 8, <a href="https://msdn.microsoft.com/f0bd649e-746d-4802-87fe-d8baec2b252f">IKEEXT_AUTHENTICATION_METHOD2</a> is available. For Windows Vista, <a href="https://msdn.microsoft.com/ce11d9ac-2636-432b-9bc7-3509f52478d9">IKEEXT_AUTHENTICATION_METHOD0</a> is available.</div>
<div> </div>



## -struct-fields




### -field authenticationMethodType

Type of authentication method specified by <a href="https://msdn.microsoft.com/582ec1ea-9390-4f86-9a3c-25d4e805a218">IKEEXT_AUTHENTICATION_METHOD_TYPE</a>.


### -field presharedKeyAuthentication

Available when <b>authenticationMethodType</b> is <b>IKEEXT_PRESHARED_KEY</b>.

See <a href="https://msdn.microsoft.com/b2009797-f5fd-4d14-8a59-832f9a0acff1">IKEEXT_PRESHARED_KEY_AUTHENTICATION1</a> for more information.


### -field certificateAuthentication

Available when <b>authenticationMethodType</b> is <b>IKEEXT_CERTIFICATE</b>, <b>IKEEXT_CERTIFICATE_ECDSA_P256</b>, or <b>IKEEXT_CERTIFICATE_ECDSA_P384</b>.

See <a href="https://msdn.microsoft.com/45325f89-b5c9-4f8c-b9b0-4f0b01b34aab">IKEEXT_CERTIFICATE_AUTHENTICATION1</a> for more information.


### -field kerberosAuthentication

Available when <b>authenticationMethodType</b> is <b>IKEEXT_KERBEROS</b>.

See <a href="https://msdn.microsoft.com/2dd626c2-4b70-450a-ad6a-a978f1d93bbf">IKEEXT_KERBEROS_AUTHENTICATION0</a> for more information.


### -field ntlmV2Authentication

Available when <b>authenticationMethodType</b> is <b>IKEEXT_NTLM_V2</b>.

See <a href="https://msdn.microsoft.com/8ac34054-5066-49f2-80b6-e674f6175c8e">IKEEXT_NTLM_V2_AUTHENTICATION0</a> for more information.


### -field sslAuthentication

Available when <b>authenticationMethodType</b> is <b>IKEEXT_SSL</b>, <b>IKEEXT_SSL_ECDSA_P256</b>, or <b>IKEEXT_SSL_ECDSA_P384</b>.

See <a href="https://msdn.microsoft.com/45325f89-b5c9-4f8c-b9b0-4f0b01b34aab">IKEEXT_CERTIFICATE_AUTHENTICATION1</a> for more information.


### -field cgaAuthentication

Available when <b>authenticationMethodType</b> is <b>IKEEXT_IPV6_CGA</b>.

See <a href="https://msdn.microsoft.com/6b472140-f3e3-45b9-81f3-9c428b687fe4">IKEEXT_IPV6_CGA_AUTHENTICATION0</a> for more information.


### -field eapAuthentication

Available when <b>authenticationMethodType</b> is <b>IKEEXT_EAP</b>.

See <a href="https://msdn.microsoft.com/86029526-ea87-4962-b5f5-f535c7034c60">IKEEXT_EAP_AUTHENTICATION0</a> for more information.


## -see-also




<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 
