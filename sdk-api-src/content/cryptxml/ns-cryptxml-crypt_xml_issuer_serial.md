---
UID: NS:cryptxml._CRYPT_XML_ISSUER_SERIAL
title: CRYPT_XML_ISSUER_SERIAL
author: windows-sdk-content
description: Contains an X.509 issued distinguished name&#8211;serial number pair.
old-location: security\crypt_xml_issuer_serial.htm
tech.root: seccrypto
ms.assetid: 8d74e119-c7ea-4c7c-9d2a-e81f7ae40310
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CRYPT_XML_ISSUER_SERIAL, CRYPT_XML_ISSUER_SERIAL structure [Security], cryptxml/CRYPT_XML_ISSUER_SERIAL, security.crypt_xml_issuer_serial
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: cryptxml.h
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
 - Cryptxml.h
api_name:
 - CRYPT_XML_ISSUER_SERIAL
product: Windows
targetos: Windows
req.typenames: CRYPT_XML_ISSUER_SERIAL
req.redist: 
---

# CRYPT_XML_ISSUER_SERIAL structure


## -description


The <b>CRYPT_XML_ISSUER_SERIAL</b> structure contains an <a href="https://msdn.microsoft.com/28dba6ef-939f-4789-9789-ee6e0fef0177">X.509</a> issued distinguished name–serial number pair.


## -struct-fields




### -field wszIssuer

A pointer to a null-terminated wide character string that contains the issuer of the certificate.


### -field wszSerial

A pointer to a null-terminated wide character string that contains the serial number of the certificate.
