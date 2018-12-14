---
UID: NS:bcrypt._BCRYPT_ECCKEY_BLOB
title: BCRYPT_ECCKEY_BLOB
author: windows-sdk-content
description: Used as a header for an elliptic curve public key or private key BLOB in memory.
old-location: security\bcrypt_ecckey_blob.htm
tech.root: seccng
ms.assetid: e60f6630-e4b0-4f35-a3cf-95dbcb007124
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PBCRYPT_ECCKEY_BLOB, BCRYPT_ECCKEY_BLOB, BCRYPT_ECCKEY_BLOB structure [Security], BCRYPT_ECDH_PRIVATE_P256_MAGIC, BCRYPT_ECDH_PRIVATE_P384_MAGIC, BCRYPT_ECDH_PRIVATE_P521_MAGIC, BCRYPT_ECDH_PUBLIC_P256_MAGIC, BCRYPT_ECDH_PUBLIC_P384_MAGIC, BCRYPT_ECDH_PUBLIC_P521_MAGIC, BCRYPT_ECDSA_PRIVATE_P256_MAGIC, BCRYPT_ECDSA_PRIVATE_P384_MAGIC, BCRYPT_ECDSA_PRIVATE_P521_MAGIC, BCRYPT_ECDSA_PUBLIC_P256_MAGIC, BCRYPT_ECDSA_PUBLIC_P384_MAGIC, BCRYPT_ECDSA_PUBLIC_P521_MAGIC, PBCRYPT_ECCKEY_BLOB, PBCRYPT_ECCKEY_BLOB structure pointer [Security], bcrypt/BCRYPT_ECCKEY_BLOB, bcrypt/PBCRYPT_ECCKEY_BLOB, security.bcrypt_ecckey_blob"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: bcrypt.h
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
 - Bcrypt.h
api_name:
 - BCRYPT_ECCKEY_BLOB
product: Windows
targetos: Windows
req.typenames: BCRYPT_ECCKEY_BLOB, *PBCRYPT_ECCKEY_BLOB
req.redist: 
---

# BCRYPT_ECCKEY_BLOB structure


## -description


The <b>BCRYPT_ECCKEY_BLOB</b> structure is used as a header for an elliptic curve <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">public key</a> or <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">private key</a> <a href="https://msdn.microsoft.com/2e570727-7da0-4e17-bf5d-6fe0e6aef65b">BLOB</a> in memory.


## -struct-fields




### -field dwMagic

 


### -field cbKey

The length, in bytes, of the key.


#### - Magic

Specifies the type of key this BLOB represents. The possible values for this member depend on the type of BLOB this structure represents. The following keys use the NIST 256-bit prime curve defined in FIPS 186-2.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDH_PUBLIC_P256_MAGIC"></a><a id="bcrypt_ecdh_public_p256_magic"></a><dl>
<dt><b>BCRYPT_ECDH_PUBLIC_P256_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 256 bit elliptic curve Diffie-Hellman public key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDH_PRIVATE_P256_MAGIC"></a><a id="bcrypt_ecdh_private_p256_magic"></a><dl>
<dt><b>BCRYPT_ECDH_PRIVATE_P256_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 256 bit elliptic curve Diffie-Hellman private key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDH_PUBLIC_P384_MAGIC"></a><a id="bcrypt_ecdh_public_p384_magic"></a><dl>
<dt><b>BCRYPT_ECDH_PUBLIC_P384_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 384 bit elliptic curve Diffie-Hellman public key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDH_PRIVATE_P384_MAGIC"></a><a id="bcrypt_ecdh_private_p384_magic"></a><dl>
<dt><b>BCRYPT_ECDH_PRIVATE_P384_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 384 bit elliptic curve Diffie-Hellman private key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDH_PUBLIC_P521_MAGIC"></a><a id="bcrypt_ecdh_public_p521_magic"></a><dl>
<dt><b>BCRYPT_ECDH_PUBLIC_P521_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 521 bit elliptic curve Diffie-Hellman public key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDH_PRIVATE_P521_MAGIC"></a><a id="bcrypt_ecdh_private_p521_magic"></a><dl>
<dt><b>BCRYPT_ECDH_PRIVATE_P521_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 521 bit elliptic curve Diffie-Hellman private key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDSA_PUBLIC_P256_MAGIC"></a><a id="bcrypt_ecdsa_public_p256_magic"></a><dl>
<dt><b>BCRYPT_ECDSA_PUBLIC_P256_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 256 bit elliptic curve DSA public key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDSA_PRIVATE_P256_MAGIC"></a><a id="bcrypt_ecdsa_private_p256_magic"></a><dl>
<dt><b>BCRYPT_ECDSA_PRIVATE_P256_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 256 bit elliptic curve DSA private key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDSA_PUBLIC_P384_MAGIC"></a><a id="bcrypt_ecdsa_public_p384_magic"></a><dl>
<dt><b>BCRYPT_ECDSA_PUBLIC_P384_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 384 bit elliptic curve DSA public key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDSA_PRIVATE_P384_MAGIC"></a><a id="bcrypt_ecdsa_private_p384_magic"></a><dl>
<dt><b>BCRYPT_ECDSA_PRIVATE_P384_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 384 bit elliptic curve DSA private key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDSA_PUBLIC_P521_MAGIC"></a><a id="bcrypt_ecdsa_public_p521_magic"></a><dl>
<dt><b>BCRYPT_ECDSA_PUBLIC_P521_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 521 bit elliptic curve DSA public key.

</td>
</tr>
<tr>
<td width="40%"><a id="BCRYPT_ECDSA_PRIVATE_P521_MAGIC"></a><a id="bcrypt_ecdsa_private_p521_magic"></a><dl>
<dt><b>BCRYPT_ECDSA_PRIVATE_P521_MAGIC</b></dt>
</dl>
</td>
<td width="60%">
The key is a 521 bit elliptic curve DSA private key.

</td>
</tr>
</table>
 


## -remarks



This structure is used as a header for a larger buffer. An elliptic curve <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">public key BLOB</a> (BCRYPT_ECCPUBLIC_BLOB) has the following format in contiguous memory. The X and Y coordinates are unsigned integers encoded in big-endian format.

<pre class="syntax" xml:space="preserve"><code>
BCRYPT_ECCKEY_BLOB
BYTE X[cbKey] // Big-endian.
BYTE Y[cbKey] // Big-endian.

</code></pre>
An elliptic curve <a href="https://msdn.microsoft.com/2fe6cfd3-8a2e-4dbe-9fb8-332633daa97a">private key BLOB</a> (BCRYPT_ECCPRIVATE_BLOB) has the following format in contiguous memory. The X and Y coordinates and d value are unsigned integers encoded in big-endian format.

<pre class="syntax" xml:space="preserve"><code>
BCRYPT_ECCKEY_BLOB
BYTE X[cbKey] // Big-endian.
BYTE Y[cbKey] // Big-endian.
BYTE d[cbKey] // Big-endian.

</code></pre>



## -see-also




<a href="https://msdn.microsoft.com/ae7e8db3-858d-4573-afe1-c9bc14d76480">BCRYPT_KEY_BLOB</a>



<a href="https://msdn.microsoft.com/a5d73143-c1d6-43b3-a724-7e27c68a5ade">BCryptExportKey</a>



<a href="https://msdn.microsoft.com/6b9683f4-10f2-40e4-9757-a1f01991bef7">BCryptImportKey</a>
 

 
