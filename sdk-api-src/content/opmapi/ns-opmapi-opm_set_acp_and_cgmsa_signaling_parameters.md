---
UID: NS:opmapi._OPM_SET_ACP_AND_CGMSA_SIGNALING_PARAMETERS
title: OPM_SET_ACP_AND_CGMSA_SIGNALING_PARAMETERS
author: windows-sdk-content
description: Contains information for the OPM_SET_ACP_AND_CGMSA_SIGNALING command in Output Protection Manager (OPM).
old-location: mf\opm_set_acp_and_cgmsa_signaling_parameters.htm
tech.root: medfound
ms.assetid: bb7caedd-cd9e-4b36-b1a1-a457de44afb1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: OPM_SET_ACP_AND_CGMSA_SIGNALING_PARAMETERS, OPM_SET_ACP_AND_CGMSA_SIGNALING_PARAMETERS structure [Media Foundation], mf.opm_set_acp_and_cgmsa_signaling_parameters, opmapi/OPM_SET_ACP_AND_CGMSA_SIGNALING_PARAMETERS
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: opmapi.h
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
 - opmapi.h
api_name:
 - OPM_SET_ACP_AND_CGMSA_SIGNALING_PARAMETERS
product: Windows
targetos: Windows
req.typenames: OPM_SET_ACP_AND_CGMSA_SIGNALING_PARAMETERS
req.redist: 
---

# OPM_SET_ACP_AND_CGMSA_SIGNALING_PARAMETERS structure


## -description


Contains information for the <a href="https://msdn.microsoft.com/ed78b7eb-bf15-4068-ab86-ae42a5e62096">OPM_SET_ACP_AND_CGMSA_SIGNALING</a> command in <a href="https://msdn.microsoft.com/daae615b-37c4-4044-91c6-693357e0016a">Output Protection Manager</a> (OPM).

This command causes the driver to insert Wide Screen Signaling (WSS) codes or other data packets in the television signal, as required by some Analog Copy Protection (ACP) and Copy Generation Management System — Analog (CGMS-A) specifications. For example:
<ul>
<li>ETSI EN 300 294 (625i PAL): Data packets are inserted into line 23 of the signal.</li>
<li>CEA-608-B (NTSC): Data packets are inserted into line 21 of the vertical blanking interval (VBI).</li>
</ul>

## -struct-fields




### -field ulNewTVProtectionStandard

Specifies the protection standard and format that is currently active. The value is a bitwise <b>OR</b> of <a href="https://msdn.microsoft.com/8f26aa92-ed40-483e-ac78-c071619f0e12">TV Protection Standard Flags</a>.


### -field ulAspectRatioChangeMask1

A bitmask indicating which bits from <b>ulAspectRatioData1</b> to set in the signal.


### -field ulAspectRatioData1

Specifies the aspect ratio value to be set for the current protection standard. For EN 300 294, use the <a href="https://msdn.microsoft.com/3c0fc524-b75f-4397-bd01-25be44062e8c">OPM_IMAGE_ASPECT_RATIO_EN300294</a> enumeration.


### -field ulAspectRatioChangeMask2

A bitmask indicating which bits from <b>ulAspectRatioData2</b> to set in the signal.


### -field ulAspectRatioData2

An additional data element related to aspect ratio. The presence and meaning of this data depends on the protection standard. This field can be used to convey End and Q0 bits for EIA-608-B, or the active format description for CEA-805-A.


### -field ulAspectRatioChangeMask3

A bitmask indicating which bits from <b>ulAspectRatioData3</b> to set in the signal.


### -field ulAspectRatioData3

An additional data element related to aspect ratio for the current protection standard. The presence and meaning of this data depends on the protection standard.


### -field ulReserved

Reserved for future use. Set the entire array to zero.


### -field ulReserved2

Reserved for future use. Set the entire array to zero.


### -field ulReserved3

Reserved for future use. Set to zero.


## -remarks



The layout of this structure is identical to the <a href="https://msdn.microsoft.com/f104b0c6-2b2f-4e6a-97e6-d73008cb80ef">DXVA_COPPSetSignalingCmdData</a> structure used in Certified Output Protection Manager (COPP).




## -see-also




<a href="https://msdn.microsoft.com/676a60ca-393e-4b5d-89d3-50cf4b771492">OPM Structures</a>



<a href="https://msdn.microsoft.com/daae615b-37c4-4044-91c6-693357e0016a">Output Protection Manager</a>
 

 
