---
UID: NS:fwpstypes.FWPS_INCOMING_VALUES0_
title: FWPS_INCOMING_VALUES0
author: windows-sdk-content
description: The FWPS_INCOMING_VALUES0 structure defines data values that are passed by the filter engine to a callout's classifyFn callout function.Note  FWPS_INCOMING_VALUES0 is a specific version of FWPS_INCOMING_VALUES.
old-location: netvista\fwps_incoming_values0.htm
tech.root: NetVista
ms.assetid: 62cec782-3d55-4bf0-a3a1-4eb2f11d5813
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FWPS_INCOMING_VALUES0, FWPS_INCOMING_VALUES0 structure [Network Drivers Starting with Windows Vista], fwpstypes/FWPS_INCOMING_VALUES0, netvista.fwps_incoming_values0, wfp_ref_3_struct_3_fwps_F-O_8a5ec685-98ff-49f2-9e78-72d409fece93.xml
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: fwpstypes.h
req.include-header: Fwpsk.h
req.target-type: Windows
req.target-min-winverclnt: Available starting with Windows Vista.
req.target-min-winversvr: 
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
 - fwpstypes.h
api_name:
 - FWPS_INCOMING_VALUES0
product: Windows
targetos: Windows
req.typenames: FWPS_INCOMING_VALUES0
req.redist: 
---

# FWPS_INCOMING_VALUES0 structure


## -description


The <b>FWPS_INCOMING_VALUES0</b> structure defines data values that are passed by the filter engine to a
  callout's 
  <a href="https://msdn.microsoft.com/e8423c27-d3eb-4bef-a835-37fae0e2b68c">classifyFn</a> callout function.
<div class="alert"><b>Note</b>  <b>FWPS_INCOMING_VALUES0</b> is a specific version of <b>FWPS_INCOMING_VALUES</b>. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a> for more information.</div><div> </div>

## -struct-fields




### -field layerId

The run-time filtering layer identifier for the filtering layer at which the data values were
     obtained. For more information, see 
     <a href="https://msdn.microsoft.com/en-us/library/windows/desktop/aa366492">Run-time Filtering Layer
     Identifiers</a>.


### -field valueCount

The number of 
     <a href="https://msdn.microsoft.com/94a81a93-7c92-4c0a-9ac7-c2085175c1a7">FWPS_INCOMING_VALUE0</a> structures in the
     array pointed to by the 
     <b>incomingValue</b> member.


### -field incomingValue

A pointer to an array of 
     <a href="https://msdn.microsoft.com/94a81a93-7c92-4c0a-9ac7-c2085175c1a7">FWPS_INCOMING_VALUE0</a> structures that
     contain the data values.


## -remarks



The filter engine passes a pointer to an FWPS_INCOMING_VALUES0 structure to a callout's 
    <a href="https://msdn.microsoft.com/e8423c27-d3eb-4bef-a835-37fae0e2b68c">classifyFn</a> callout function.




## -see-also




<a href="https://msdn.microsoft.com/94a81a93-7c92-4c0a-9ac7-c2085175c1a7">FWPS_INCOMING_VALUE0</a>



<a href="https://msdn.microsoft.com/e8423c27-d3eb-4bef-a835-37fae0e2b68c">classifyFn</a>
 

 
