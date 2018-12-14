---
UID: NS:wincrypt._CRL_FIND_ISSUED_FOR_PARA
title: CRL_FIND_ISSUED_FOR_PARA
author: windows-sdk-content
description: Contains the certificate contexts of both a subject and a certificate issuer.
old-location: security\crl_find_issued_for_para.htm
tech.root: seccrypto
ms.assetid: a5c04859-00bb-4b7d-a98c-5b17bf0fa38a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCRL_FIND_ISSUED_FOR_PARA, CRL_FIND_ISSUED_FOR_PARA, CRL_FIND_ISSUED_FOR_PARA structure [Security], PCRL_FIND_ISSUED_FOR_PARA, PCRL_FIND_ISSUED_FOR_PARA structure pointer [Security], _crypto2_crl_find_issued_for_para, security.crl_find_issued_for_para, wincrypt/CRL_FIND_ISSUED_FOR_PARA, wincrypt/PCRL_FIND_ISSUED_FOR_PARA"
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
 - CRL_FIND_ISSUED_FOR_PARA
product: Windows
targetos: Windows
req.typenames: CRL_FIND_ISSUED_FOR_PARA, *PCRL_FIND_ISSUED_FOR_PARA
req.redist: 
---

# CRL_FIND_ISSUED_FOR_PARA structure


## -description


The <b>CRL_FIND_ISSUED_FOR_PARA</b> structure contains the certificate contexts of both a subject and a certificate issuer. For more information, see 
<a href="https://msdn.microsoft.com/3e481912-204a-4d86-ab67-81f8ae4d1aaa">CertFindCRLInStore</a>.


## -struct-fields




### -field pSubjectCert

A pointer to a subject's certificate context.


### -field pIssuerCert

A pointer to a certificate issuer's certificate context.
