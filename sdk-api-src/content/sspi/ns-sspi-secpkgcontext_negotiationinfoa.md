---
UID: NS:sspi._SecPkgContext_NegotiationInfoA
title: SecPkgContext_NegotiationInfoA
author: windows-sdk-content
description: The SecPkgContext_NegotiationInfo structure contains information on the security package that is being set up or has been set up, and also gives the status on the negotiation to set up the security package.
old-location: security\secpkgcontext_negotiationinfo.htm
tech.root: secauthn
ms.assetid: 3af724b8-fbe5-4a75-b128-9efe65381f2f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSecPkgContext_NegotiationInfoA, PSecPkgContext_NegotiationInfo, PSecPkgContext_NegotiationInfo structure pointer [Security], SECPKG_NEGOTIATION_COMPLETE, SECPKG_NEGOTIATION_IN_PROGRESS, SECPKG_NEGOTIATION_OPTIMISTIC, SecPkgContext_NegotiationInfo, SecPkgContext_NegotiationInfo structure [Security], SecPkgContext_NegotiationInfoA, SecPkgContext_NegotiationInfoW, _ssp_secpkgcontext_negotiationinfo, security.secpkgcontext_negotiationinfo, sspi/PSecPkgContext_NegotiationInfo, sspi/SecPkgContext_NegotiationInfo, sspi/SecPkgContext_NegotiationInfoA, sspi/SecPkgContext_NegotiationInfoW"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: sspi.h
req.include-header: Security.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SecPkgContext_NegotiationInfoW (Unicode) and SecPkgContext_NegotiationInfoA (ANSI)
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
 - SecPkgContext_NegotiationInfo
 - SecPkgContext_NegotiationInfoA
 - SecPkgContext_NegotiationInfoW
product: Windows
targetos: Windows
req.typenames: SecPkgContext_NegotiationInfoA, *PSecPkgContext_NegotiationInfoA
req.redist: 
---

# SecPkgContext_NegotiationInfoA structure


## -description


The <b>SecPkgContext_NegotiationInfo</b> structure contains information on the <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security package</a> that is being set up or has been set up, and also gives the status on the negotiation to set up the security package.


## -struct-fields




### -field PackageInfo

Pointer to a 
<a href="https://msdn.microsoft.com/d0bff3d8-63f1-4a4e-851f-177040af6bd2">SecPkgInfo</a> structure that provides general information about the security package chosen in the negotiate process, such as the name and capabilities of the package.


### -field NegotiationState

Indicator of the state of the negotiation for the security package identified in the <b>PackageInfo</b> member. This attribute can be queried from the context handle before the setup is complete, such as when ISC returns SEC_I_CONTINUE_NEEDED.

The following table shows values returned in this member.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="SECPKG_NEGOTIATION_COMPLETE"></a><a id="secpkg_negotiation_complete"></a><dl>
<dt><b>SECPKG_NEGOTIATION_COMPLETE</b></dt>
</dl>
</td>
<td width="60%">
Negotiation has been completed.

</td>
</tr>
<tr>
<td width="40%"><a id="SECPKG_NEGOTIATION_OPTIMISTIC"></a><a id="secpkg_negotiation_optimistic"></a><dl>
<dt><b>SECPKG_NEGOTIATION_OPTIMISTIC</b></dt>
</dl>
</td>
<td width="60%">
Negotiations not yet completed.

</td>
</tr>
<tr>
<td width="40%"><a id="SECPKG_NEGOTIATION_IN_PROGRESS"></a><a id="secpkg_negotiation_in_progress"></a><dl>
<dt><b>SECPKG_NEGOTIATION_IN_PROGRESS</b></dt>
</dl>
</td>
<td width="60%">
Negotiations in progress.

</td>
</tr>
</table>
 
