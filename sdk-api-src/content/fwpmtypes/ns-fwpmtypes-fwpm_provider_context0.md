---
UID: NS:fwpmtypes.FWPM_PROVIDER_CONTEXT0_
title: FWPM_PROVIDER_CONTEXT0
author: windows-sdk-content
description: Stores the state associated with a provider context.
old-location: fwp\fwpm_provider_context0_struct.htm
tech.root: fwp
ms.assetid: 99105044-f4fa-42f2-8393-f0ee8948e9ff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FWPM_PROVIDER_CONTEXT0, FWPM_PROVIDER_CONTEXT0 structure [Filtering], FWPM_PROVIDER_CONTEXT0_, FWPM_PROVIDER_CONTEXT_FLAG_PERSISTENT, fwp.fwpm_provider_context0_struct, fwpmtypes/FWPM_PROVIDER_CONTEXT0
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: fwpmtypes.h
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
 - Fwpmtypes.h
api_name:
 - FWPM_PROVIDER_CONTEXT0
product: Windows
targetos: Windows
req.typenames: FWPM_PROVIDER_CONTEXT0
req.redist: 
---

# FWPM_PROVIDER_CONTEXT0 structure


## -description


The <b>FWPM_PROVIDER_CONTEXT0</b> structure stores the state associated with a provider context.
<div class="alert"><b>Note</b>  <b>FWPM_PROVIDER_CONTEXT0</b> is the specific implementation of FWPM_PROVIDER_CONTEXT used in Windows Vista. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows 7, <a href="https://msdn.microsoft.com/34727579-9baf-4d50-b973-e864ddf651b0">FWPM_PROVIDER_CONTEXT1</a> is available. For Windows 8, <a href="https://msdn.microsoft.com/aa397a4e-07cc-4eee-8d0f-798901a5bb29">FWPM_PROVIDER_CONTEXT2</a> is available. </div><div> </div>

## -struct-fields




### -field providerContextKey

Uniquely identifies the provider context. If the GUID is zero-initialized
   in the call to <a href="https://msdn.microsoft.com/c31595b8-81e4-4399-b2a3-d228c35875fe">FwpmProviderContextAdd0</a>, Base Filtering Engine (BFE) will generate one.


### -field displayData

Allows provider contexts to be annotated in a human-readable form. The <b>name</b> member of the <a href="https://msdn.microsoft.com/b86ca572-b4f4-4d40-adfd-fb0e9d32fcd5">FWPM_DISPLAY_DATA0</a> structure is required.


### -field flags

Possible values:

<table>
<tr>
<th>Provider context flag</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="FWPM_PROVIDER_CONTEXT_FLAG_PERSISTENT"></a><a id="fwpm_provider_context_flag_persistent"></a><dl>
<dt><b>FWPM_PROVIDER_CONTEXT_FLAG_PERSISTENT</b></dt>
</dl>
</td>
<td width="60%">
The object is persistent, that is, it survives across BFE stop/start.

</td>
</tr>
</table>
 


### -field providerKey

GUID of the policy provider that manages this object.


### -field providerData

An <a href="https://msdn.microsoft.com/85f360bf-5ee4-4980-b4ce-15ff310d8fbe">FWP_BYTE_BLOB</a> structure that contains optional provider-specific data that allows providers to store additional context info with the object.


### -field type

A <a href="https://msdn.microsoft.com/e8eae5e7-9240-47a5-851b-1ec51cb07b63">FWPM_PROVIDER_CONTEXT_TYPE</a> value specifying the type of provider context..


### -field keyingPolicy

Available when <b>type</b> is <b>FWPM_IPSEC_KEYING_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/6eddafbf-ac57-419f-b2a0-f50a4ab31baf">IPSEC_KEYING_POLICY0</a> for more information.


### -field ikeQmTransportPolicy

Available when <b>type</b> is <b>FWPM_IPSEC_IKE_QM_TRANSPORT_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/c17ebe74-41e3-467c-875a-db43978a5234">IPSEC_TRANSPORT_POLICY0</a> for more information.


### -field ikeQmTunnelPolicy

Available when <b>type</b> is <b>FWPM_IPSEC_IKE_QM_TUNNEL_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/092b108c-47e1-4b2f-b7ed-184cf8abb392">IPSEC_TUNNEL_POLICY0</a> for more information.


### -field authipQmTransportPolicy

Available when <b>type</b> is <b>FWPM_IPSEC_AUTHIP_QM_TRANSPORT_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/c17ebe74-41e3-467c-875a-db43978a5234">IPSEC_TRANSPORT_POLICY0</a> for more information.


### -field authipQmTunnelPolicy

Available when <b>type</b> is <b>FWPM_IPSEC_AUTHIP_QM_TUNNEL_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/092b108c-47e1-4b2f-b7ed-184cf8abb392">IPSEC_TUNNEL_POLICY0</a> for more information.


### -field ikeMmPolicy

Available when <b>type</b> is <b>FWPM_IPSEC_IKE_MM_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/4c33087a-2736-491c-a89f-e4b9ab136026">IKEEXT_POLICY0</a> for more information.


### -field authIpMmPolicy

Available when <b>type</b> is <b>FWPM_IPSEC_AUTHIP_MM_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/4c33087a-2736-491c-a89f-e4b9ab136026">IKEEXT_POLICY0</a> for more information.


### -field dataBuffer

Available when <b>type</b> is <b>FWPM_GENERAL_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/85f360bf-5ee4-4980-b4ce-15ff310d8fbe">FWP_BYTE_BLOB</a> for more information.


### -field classifyOptions

Available when <b>type</b> is <b>FWPM_CLASSIFY_OPTIONS_CONTEXT</b>.

See <a href="https://msdn.microsoft.com/5d1f7807-4188-4a57-83fc-99683254e3a5">FWPM_CLASSIFY_OPTIONS0</a> for more information.


### -field providerContextId

LUID identifying the context.  This is the context value stored in the <b>FWPS_FILTER0</b> structure for filters that reference a provider context. The <b>FWPS_FILTER0</b> structure is documented in the WDK.


## -remarks



The first seven elements of the union are information supplied when adding objects.

The last element is additional information returned when getting/enumerating objects.




## -see-also




<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 
