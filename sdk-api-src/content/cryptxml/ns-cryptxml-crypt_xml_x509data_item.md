---
UID: NS:cryptxml._CRYPT_XML_X509DATA_ITEM
title: CRYPT_XML_X509DATA_ITEM
author: windows-sdk-content
description: Represents X.509 data that is to be encoded in an X509Data named element.
old-location: security\crypt_xml_x509data_item.htm
tech.root: seccrypto
ms.assetid: 118371c7-9b75-4330-9897-bd352b072fa4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CRYPT_XML_X509DATA_ITEM, CRYPT_XML_X509DATA_ITEM structure [Security], CRYPT_XML_X509DATA_TYPE_CERTIFICATE, CRYPT_XML_X509DATA_TYPE_CRL, CRYPT_XML_X509DATA_TYPE_CUSTOM, CRYPT_XML_X509DATA_TYPE_ISSUER_SERIAL, CRYPT_XML_X509DATA_TYPE_SKI, CRYPT_XML_X509DATA_TYPE_SUBJECT_NAME, cryptxml/CRYPT_XML_X509DATA_ITEM, security.crypt_xml_x509data_item
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
 - CRYPT_XML_X509DATA_ITEM
product: Windows
targetos: Windows
req.typenames: CRYPT_XML_X509DATA_ITEM
req.redist: 
---

# CRYPT_XML_X509DATA_ITEM structure


## -description


The <b>CRYPT_XML_X509DATA_ITEM</b> structure represents  <a href="https://msdn.microsoft.com/28dba6ef-939f-4789-9789-ee6e0fef0177">X.509</a> data that is to be encoded in an X509Data named element.


## -struct-fields




### -field dwType

Specifies the data item type. 


This member can be one of the following values.



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="CRYPT_XML_X509DATA_TYPE_ISSUER_SERIAL"></a><a id="crypt_xml_x509data_type_issuer_serial"></a><dl>
<dt><b>CRYPT_XML_X509DATA_TYPE_ISSUER_SERIAL</b></dt>
<dt>0x00000001</dt>
</dl>
</td>
<td width="60%">
The X.509 data is an issuer serial number.

</td>
</tr>
<tr>
<td width="40%"><a id="CRYPT_XML_X509DATA_TYPE_SKI"></a><a id="crypt_xml_x509data_type_ski"></a><dl>
<dt><b>CRYPT_XML_X509DATA_TYPE_SKI</b></dt>
<dt>0x00000002</dt>
</dl>
</td>
<td width="60%">
The X.509 data is a Subject Key Identifier (SKI).

</td>
</tr>
<tr>
<td width="40%"><a id="CRYPT_XML_X509DATA_TYPE_SUBJECT_NAME"></a><a id="crypt_xml_x509data_type_subject_name"></a><dl>
<dt><b>CRYPT_XML_X509DATA_TYPE_SUBJECT_NAME</b></dt>
<dt>0x00000003</dt>
</dl>
</td>
<td width="60%">
The X.509 data is a subject name.

</td>
</tr>
<tr>
<td width="40%"><a id="CRYPT_XML_X509DATA_TYPE_CERTIFICATE"></a><a id="crypt_xml_x509data_type_certificate"></a><dl>
<dt><b>CRYPT_XML_X509DATA_TYPE_CERTIFICATE</b></dt>
<dt>0x00000004</dt>
</dl>
</td>
<td width="60%">
The X.509 data is a certificate.

</td>
</tr>
<tr>
<td width="40%"><a id="CRYPT_XML_X509DATA_TYPE_CRL"></a><a id="crypt_xml_x509data_type_crl"></a><dl>
<dt><b>CRYPT_XML_X509DATA_TYPE_CRL</b></dt>
<dt>0x00000005</dt>
</dl>
</td>
<td width="60%">
The X.509 data is a <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certificate revocation list</a> (CRL).

</td>
</tr>
<tr>
<td width="40%"><a id="CRYPT_XML_X509DATA_TYPE_CUSTOM"></a><a id="crypt_xml_x509data_type_custom"></a><dl>
<dt><b>CRYPT_XML_X509DATA_TYPE_CUSTOM</b></dt>
<dt>0x00000006</dt>
</dl>
</td>
<td width="60%">
The X.509 data is a custom format.

</td>
</tr>
</table>
 


### -field IssuerSerial

A <a href="https://msdn.microsoft.com/8d74e119-c7ea-4c7c-9d2a-e81f7ae40310">CRYPT_XML_ISSUER_SERIAL</a> structure that contains serial number data.


### -field SKI

A <a href="https://msdn.microsoft.com/dc7e23d6-923c-40d2-9cf7-9a529c0634ce">CRYPT_XML_DATA_BLOB</a> structure that contains SKI data.


### -field wszSubjectName

A pointer to a null-terminated Unicode string that contains the subject name.


### -field Certificate

A <a href="https://msdn.microsoft.com/dc7e23d6-923c-40d2-9cf7-9a529c0634ce">CRYPT_XML_DATA_BLOB</a> structure that contains certificate data.


### -field CRL

A <a href="https://msdn.microsoft.com/dc7e23d6-923c-40d2-9cf7-9a529c0634ce">CRYPT_XML_DATA_BLOB</a> that contains a CRL.


### -field Custom

A <a href="https://msdn.microsoft.com/b70aae53-919b-4d4a-b284-ea6bc223842f">CRYPT_XML_BLOB</a> structure that contains custom data.
