---
UID: NE:imapi2._IMAPI_BURN_VERIFICATION_LEVEL
title: IMAPI_BURN_VERIFICATION_LEVEL
author: windows-sdk-content
description: Defines values for the burn verification implemented by the IBurnVerification interface.
old-location: imapi\imapi_burn_verification_level.htm
tech.root: imapi
ms.assetid: 83a267b7-8b25-49b8-b1d0-83efbad8fa2a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PIMAPI_BURN_VERIFICATION_LEVEL, IMAPI_BURN_VERIFICATION_FULL, IMAPI_BURN_VERIFICATION_LEVEL, IMAPI_BURN_VERIFICATION_LEVEL enumeration [IMAPI], IMAPI_BURN_VERIFICATION_NONE, IMAPI_BURN_VERIFICATION_QUICK, imapi.imapi_burn_verification_level, imapi2/IMAPI_BURN_VERIFICATION_FULL, imapi2/IMAPI_BURN_VERIFICATION_LEVEL, imapi2/IMAPI_BURN_VERIFICATION_NONE, imapi2/IMAPI_BURN_VERIFICATION_QUICK"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: imapi2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Imapi2.idl
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
 - imapi2.h
api_name:
 - IMAPI_BURN_VERIFICATION_LEVEL
product: Windows
targetos: Windows
req.typenames: IMAPI_BURN_VERIFICATION_LEVEL, *PIMAPI_BURN_VERIFICATION_LEVEL
req.redist: 
---

# IMAPI_BURN_VERIFICATION_LEVEL enumeration


## -description


Defines values for the burn verification implemented by the <a href="https://msdn.microsoft.com/3a410ab8-dfc3-4c30-a198-3888ed750a6d">IBurnVerification</a> interface.


## -enum-fields




### -field IMAPI_BURN_VERIFICATION_NONE

No burn verification.


### -field IMAPI_BURN_VERIFICATION_QUICK

A quick, heuristic burn verification.


### -field IMAPI_BURN_VERIFICATION_FULL

This verification compares the checksum to the referenced stream for either the last session or each track.  A full verification includes the heuristic checks of a quick verification for both burn formats.


## -remarks



Depending on the format used for the burned media, the values defined by this enumeration will elicit the following behavior during verification:

<table>
<tr>
<th>MsftDiscFormat2Data</th>
<th></th>
</tr>
<tr>
<td>None</td>
<td>
No burn verification.

</td>
</tr>
<tr>
<td>Quick Verification</td>
<td>
<ul>
<li>READ_DISC_INFO command works and data appears correct</li>
<li>READ_TRACK_INFO command works on all tracks</li>
<li>Checksum comparison of a small set of disc sectors to stream bits</li>
</ul>
</td>
</tr>
<tr>
<td>Full Verification</td>
<td>
<ul>
<li>Performs the  same heuristic checks as the 'Quick' method, but will also read the entire last session and compare a checksum to the burned stream.</li>
</ul>
</td>
</tr>
</table>
 


<table>
<tr>
<th>MsftDiscFormat2TrackAtOnce</th>
<th></th>
</tr>
<tr>
<td>None</td>
<td>
No burn verification.

</td>
</tr>
<tr>
<td>Quick Verification</td>
<td>
After adding each track:

<ul>
<li>READ_TRACK_INFO command for last track appears correct</li>
</ul>
When finishing the disc:

<ul>
<li>READ_DISC_INFO command appears correct</li>
<li>TOC appears correct</li>
</ul>
</td>
</tr>
<tr>
<td>Full Verification</td>
<td>
Full verification is not supported with this format.

</td>
</tr>
</table>
 



The time required for a full verification is relative to the read speed of the device and  storage medium.

This enumeration is supported in Windows Server 2003 with Service Pack 1 (SP1), Windows XP with Service Pack 2 (SP2),  and Windows Vista  via the <a href="http://go.microsoft.com/fwlink/p/?linkid=141659">Windows Feature Pack for Storage</a>. All  features provided by this  update package are supported natively in Windows 7 and Windows Server 2008 R2.




## -see-also




<a href="https://msdn.microsoft.com/3a410ab8-dfc3-4c30-a198-3888ed750a6d">IBurnVerfication</a>
 

 
