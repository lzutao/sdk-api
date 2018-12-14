---
UID: NS:wincrypt._CERT_POLICY_MAPPING
title: CERT_POLICY_MAPPING
author: windows-sdk-content
description: Contains a mapping between issuer domain and subject domain policy OIDs.
old-location: security\cert_policy_mapping.htm
tech.root: seccrypto
ms.assetid: 6270888a-1c61-472d-8ec7-10c24b890220
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCERT_POLICY_MAPPING, CERT_POLICY_MAPPING, CERT_POLICY_MAPPING structure [Security], PCERT_POLICY_MAPPING, PCERT_POLICY_MAPPING structure pointer [Security], _crypto2_cert_policy_mapping, security.cert_policy_mapping, wincrypt/CERT_POLICY_MAPPING, wincrypt/PCERT_POLICY_MAPPING"
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
 - CERT_POLICY_MAPPING
product: Windows
targetos: Windows
req.typenames: CERT_POLICY_MAPPING, *PCERT_POLICY_MAPPING
req.redist: 
---

# CERT_POLICY_MAPPING structure


## -description


The <b>CERT_POLICY_MAPPING</b> structure contains a mapping between issuer domain and subject domain policy OIDs.


## -struct-fields




### -field pszIssuerDomainPolicy

<b>pszObjId</b> of an issuer domain policy.


### -field pszSubjectDomainPolicy

<b>pszObjId</b> of the equivalent subject domain policy.
