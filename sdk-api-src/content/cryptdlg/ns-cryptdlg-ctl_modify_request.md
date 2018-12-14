---
UID: NS:cryptdlg._CTL_MODIFY_REQUEST
title: CTL_MODIFY_REQUEST
author: windows-sdk-content
description: Contains a request to modify a certificate trust list (CTL). This structure is used in the CertModifyCertificatesToTrust function.
old-location: security\ctl_modify_request.htm
tech.root: seccrypto
ms.assetid: b8b5fd3e-a0db-4edd-84c7-48bae9adc3f8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PCTL_MODIFY_REQUEST, CTL_MODIFY_REQUEST, CTL_MODIFY_REQUEST structure [Security], CTL_MODIFY_REQUEST_ADD_NOT_TRUSTED, CTL_MODIFY_REQUEST_ADD_TRUSTED, CTL_MODIFY_REQUEST_REMOVE, PCTL_MODIFY_REQUEST, PCTL_MODIFY_REQUEST structure pointer [Security], cryptdlg/CTL_MODIFY_REQUEST, cryptdlg/PCTL_MODIFY_REQUEST, security.ctl_modify_request"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: cryptdlg.h
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
 - CryptDlg.h
api_name:
 - CTL_MODIFY_REQUEST
product: Windows
targetos: Windows
req.typenames: CTL_MODIFY_REQUEST, *PCTL_MODIFY_REQUEST
req.redist: 
---

# CTL_MODIFY_REQUEST structure


## -description


The <b>CTL_MODIFY_REQUEST</b> structure contains a request to modify a certificate trust list (CTL).  This structure is used in the <a href="https://msdn.microsoft.com/a23d968e-113f-470e-a629-18c22882c77f">CertModifyCertificatesToTrust</a> function.


## -struct-fields




### -field pccert

A pointer to a <a href="https://msdn.microsoft.com/f0a3200e-6541-423d-a4a3-595a31026eea">CERT_CONTEXT</a> structure that contains the certificate to change the trust on.


### -field dwOperation

The operation to be performed. This member can be one of the following values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="CTL_MODIFY_REQUEST_ADD_TRUSTED"></a><a id="ctl_modify_request_add_trusted"></a><dl>
<dt><b>CTL_MODIFY_REQUEST_ADD_TRUSTED</b></dt>
</dl>
</td>
<td width="60%">
Add the certificate to the CTL. The certificate is explicitly trusted.

</td>
</tr>
<tr>
<td width="40%"><a id="CTL_MODIFY_REQUEST_ADD_NOT_TRUSTED"></a><a id="ctl_modify_request_add_not_trusted"></a><dl>
<dt><b>CTL_MODIFY_REQUEST_ADD_NOT_TRUSTED</b></dt>
</dl>
</td>
<td width="60%">
 Add the certificate to the Untrusted Certificates certificate store. 
							The certificate is explicitly not trusted.

</td>
</tr>
<tr>
<td width="40%"><a id="CTL_MODIFY_REQUEST_REMOVE"></a><a id="ctl_modify_request_remove"></a><dl>
<dt><b>CTL_MODIFY_REQUEST_REMOVE</b></dt>
</dl>
</td>
<td width="60%">
Remove the certificate from the CTL. The certificate is neither explicitly trusted nor untrusted.  To be trusted, the certificate must have a trusted root certificate at the root of its certificate chain.

</td>
</tr>
</table>
 


### -field dwError

The error code generated for this operation.


## -see-also




<a href="https://msdn.microsoft.com/a23d968e-113f-470e-a629-18c22882c77f">CertModifyCertificatesToTrust</a>
 

 
