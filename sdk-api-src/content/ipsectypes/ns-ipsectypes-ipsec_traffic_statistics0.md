---
UID: NS:ipsectypes.IPSEC_TRAFFIC_STATISTICS0_
title: IPSEC_TRAFFIC_STATISTICS0
author: windows-sdk-content
description: Stores IPsec traffic statistics.
old-location: fwp\ipsec_traffic_statistics0_struct.htm
tech.root: fwp
ms.assetid: 70f67966-0ced-49a7-9d27-6976ee0bd89c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IPSEC_TRAFFIC_STATISTICS0, IPSEC_TRAFFIC_STATISTICS0 structure [Filtering], fwp.ipsec_traffic_statistics0_struct, ipsectypes/IPSEC_TRAFFIC_STATISTICS0
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ipsectypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Ipsectypes.idl
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
 - Ipsectypes.h
api_name:
 - IPSEC_TRAFFIC_STATISTICS0
product: Windows
targetos: Windows
req.typenames: IPSEC_TRAFFIC_STATISTICS0
req.redist: 
---

# IPSEC_TRAFFIC_STATISTICS0 structure


## -description


The <b>IPSEC_TRAFFIC_STATISTICS0</b> structure stores IPsec traffic statistics.
<div class="alert"><b>Note</b>  <b>IPSEC_TRAFFIC_STATISTICS0</b> is the specific implementation of IPSEC_TRAFFIC_STATISTICS used in Windows Vista. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information. For Windows 7 and later, <a href="https://msdn.microsoft.com/3b25d98a-9216-4e74-91fc-cc8658e12d9b">IPSEC_TRAFFIC_STATISTICS1</a> is available.</div><div> </div>

## -struct-fields




### -field encryptedByteCount

Specifies encrypted byte count.


### -field authenticatedAHByteCount

Specifies authenticated AH byte count.


### -field authenticatedESPByteCount

Specifies authenticated ESP byte count.


### -field transportByteCount

Specifies transport byte count.


### -field tunnelByteCount

Specifies tunnel byte count.


### -field offloadByteCount

Specifies offload byte count.


## -see-also




<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 
