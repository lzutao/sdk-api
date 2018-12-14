---
UID: NS:eaphostpeertypes._EAPHOST_AUTH_INFO
title: EAPHOST_AUTH_INFO
author: windows-sdk-content
description: Describes current authentication information throughout different stages of the EAP authentication process.
old-location: eaphost\eaphost_auth_info.htm
tech.root: eaphost
ms.assetid: b05a1862-9709-4459-a445-5ea4e00cab88
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EAPHOST_AUTH_INFO, EAPHOST_AUTH_INFO structure [EAPHost], eaphost.eaphost_auth_info, eaphostpeertypes/EAPHOST_AUTH_INFO
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: eaphostpeertypes.h
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
 - eaphostpeertypes.h
api_name:
 - EAPHOST_AUTH_INFO
product: Windows
targetos: Windows
req.typenames: EAPHOST_AUTH_INFO
req.redist: 
---

# EAPHOST_AUTH_INFO structure


## -description


 The <b>EAPHOST_AUTH_INFO</b> structure describes current authentication information throughout different stages of the EAP authentication process.


## -struct-fields




### -field status

An <a href="https://msdn.microsoft.com/e1d0ff30-955c-4998-ae01-5dbadf3f4123">EAPHOST_AUTH_STATUS</a> enumeration value that specifies the current status of the authentication session.


### -field dwErrorCode

An error value, either from winerror.h or elsewhere (Raserror.h), that indicates the last error raised during the authentication process.


### -field dwReasonCode

A reason code that specifies the reason the error in <b>dwErrorCode</b> was raised. 


## -see-also




<a href="https://msdn.microsoft.com/77595f36-140d-4d8e-af8e-63e9de0031c4">EAPHost Supplicant Structures</a>



<a href="https://msdn.microsoft.com/adbb08d7-36a0-4e10-b0bc-2fb7030c2fcc">EapHostPeerAuthParams</a>



<a href="https://msdn.microsoft.com/cb5ceffb-941f-48ad-9271-111f41adc65b">EapHostPeerGetAuthStatus</a>
 

 
