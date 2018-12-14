---
UID: NS:qossp._RSVP_ADSPEC
title: RSVP_ADSPEC
author: windows-sdk-content
description: The QOS object RSVP_ADSPEC provides a means by which information describing network devices along the data path between sender and receiver, pertaining to RSVP functionality and available services, is provided or retrieved.
old-location: qos\rsvp_adspec.htm
tech.root: QOS
ms.assetid: 90fad5de-7105-4126-a6db-d4fb663e01f4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPRSVP_ADSPEC, LPRSVP_ADSPEC, LPRSVP_ADSPEC structure pointer [QOS], RSVP_ADSPEC, RSVP_ADSPEC structure [QOS], _gqos_rsvp_adspec, qos.rsvp_adspec, qossp/LPRSVP_ADSPEC, qossp/RSVP_ADSPEC"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: qossp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - Qossp.h
api_name:
 - RSVP_ADSPEC
product: Windows
targetos: Windows
req.typenames: RSVP_ADSPEC, *LPRSVP_ADSPEC
req.redist: 
---

# RSVP_ADSPEC structure


## -description


<p class="CCE_Message">[The RSVP_ADSPEC QOS object is not supported except on Windows 2000. RSVP signaling is not supported except on Windows 2000.]

The QOS object 
<b>RSVP_ADSPEC</b> provides a means by which information describing network devices along the data path between sender and receiver, pertaining to RSVP functionality and available services, is provided or retrieved.


## -struct-fields




### -field ObjectHdr

The QOS object 
<b>QOS_OBJECT_HDR</b>.


### -field GeneralParams

An <a href="https://msdn.microsoft.com/eab6b317-9d06-45e2-bc77-0882f40e7d79">AD_GENERAL_PARAMS</a> structure that provides general characterization parameters for the flow. Information includes RSVP-enabled hop count, bandwidth and latency estimates, and the path's MTU.


### -field NumberOfServices

Provides a count of the number of services available.


### -field Services

A <a href="https://msdn.microsoft.com/604d7be8-955b-40a3-9cb4-6cbfbeeaa105">CONTROL_SERVICE</a> array, its element count based on <b>NumberOfServices</b>, which provides information about the services available along the data path between the sender and receiver of a given flow.


## -see-also




<a href="https://msdn.microsoft.com/a2021d70-e7ef-4c2a-8800-1a1d7540ce02">QOS_OBJECT_HDR</a>
 

 
