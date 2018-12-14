---
UID: NS:ntmsapi._NTMS_STORAGESLOTINFORMATION
title: NTMS_STORAGESLOTINFORMATION
author: windows-sdk-content
description: The NTMS_STORAGESLOTINFORMATION structure defines properties specific to a storage slot object.
old-location: fs\ntms_storageslotinformation.htm
tech.root: Rsm
ms.assetid: 95b9d2e9-ddf3-459f-b9de-cefc15adb419
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: NTMS_SLOTSTATE_EMPTY, NTMS_SLOTSTATE_FULL, NTMS_SLOTSTATE_NEEDSINVENTORY, NTMS_SLOTSTATE_NOTPRESENT, NTMS_SLOTSTATE_UNKNOWN, NTMS_STORAGEINFORMATION, NTMS_STORAGEINFORMATION structure [Files], NTMS_STORAGESLOTINFORMATION, NTMS_STORAGESLOTINFORMATION structure [Files], _zaw_ntms_storageslotinformation, base.ntms_storageslotinformation, fs.ntms_storageslotinformation, ntmsapi/NTMS_STORAGESLOTINFORMATION
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ntmsapi.h
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
 - Ntmsapi.h
api_name:
 - NTMS_STORAGEINFORMATION
product: Windows
targetos: Windows
req.typenames: NTMS_STORAGESLOTINFORMATION
req.redist: 
---

# NTMS_STORAGESLOTINFORMATION structure


## -description


<p class="CCE_Message">[<a href="https://msdn.microsoft.com/af7186f8-7921-48e3-a4fd-23259a6e9018">Removable Storage Manager</a> is no longer available as of Windows 7 and  Windows Server 2008 R2.]

The 
<b>NTMS_STORAGESLOTINFORMATION</b> structure defines properties specific to a storage slot object.


## -struct-fields




### -field Number

Number of the slot in the library.


### -field State

Current state of the slot. This can be one of the following values. 



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="NTMS_SLOTSTATE_EMPTY"></a><a id="ntms_slotstate_empty"></a><dl>
<dt><b>NTMS_SLOTSTATE_EMPTY</b></dt>
</dl>
</td>
<td width="60%">
Slot is present, but does not contain a piece of physical media.

</td>
</tr>
<tr>
<td width="40%"><a id="NTMS_SLOTSTATE_FULL"></a><a id="ntms_slotstate_full"></a><dl>
<dt><b>NTMS_SLOTSTATE_FULL</b></dt>
</dl>
</td>
<td width="60%">
Slot is present and contains a piece of physical media.

</td>
</tr>
<tr>
<td width="40%"><a id="NTMS_SLOTSTATE_NOTPRESENT"></a><a id="ntms_slotstate_notpresent"></a><dl>
<dt><b>NTMS_SLOTSTATE_NOTPRESENT</b></dt>
</dl>
</td>
<td width="60%">
Slot is not present. If the library contains magazines, this value is reported for each slot when the associated magazine is missing.

</td>
</tr>
<tr>
<td width="40%"><a id="NTMS_SLOTSTATE_UNKNOWN"></a><a id="ntms_slotstate_unknown"></a><dl>
<dt><b>NTMS_SLOTSTATE_UNKNOWN</b></dt>
</dl>
</td>
<td width="60%">
Slot state cannot be determined.

</td>
</tr>
<tr>
<td width="40%"><a id="NTMS_SLOTSTATE_NEEDSINVENTORY"></a><a id="ntms_slotstate_needsinventory"></a><dl>
<dt><b>NTMS_SLOTSTATE_NEEDSINVENTORY</b></dt>
</dl>
</td>
<td width="60%">
Slot needs inventory.

</td>
</tr>
</table>
 


### -field Library

Library that contains the slot.


## -remarks



The 
<b>NTMS_STORAGESLOTINFORMATION</b> structure is part of the 
<a href="https://msdn.microsoft.com/56e3380b-47c7-4861-bb2b-31d67ac10fe1">NTMS_OBJECTINFORMATION</a> structure.




## -see-also




<a href="https://msdn.microsoft.com/56e3380b-47c7-4861-bb2b-31d67ac10fe1">NTMS_OBJECTINFORMATION</a>
 

 
