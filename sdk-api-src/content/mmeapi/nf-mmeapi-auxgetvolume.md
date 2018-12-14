---
UID: NF:mmeapi.auxGetVolume
title: auxGetVolume function
author: windows-sdk-content
description: The auxGetVolume function retrieves the current volume setting of the specified auxiliary output device.
old-location: multimedia\auxgetvolume.htm
tech.root: Multimedia
ms.assetid: a427cdb5-83ec-4529-847d-1494118ef926
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "_win32_auxGetVolume, auxGetVolume, auxGetVolume function [Windows Multimedia], mmeapi/auxGetVolume, multimedia.auxgetvolume"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: mmeapi.h
req.include-header: Windows.h
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
req.lib: Winmm.lib
req.dll: Winmm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Winmm.dll
 - API-MS-Win-mm-mme-l1-1-0.dll
 - winmmbase.dll
api_name:
 - auxGetVolume
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# auxGetVolume function


## -description



The <b>auxGetVolume</b> function retrieves the current volume setting of the specified auxiliary output device.




## -parameters




### -param uDeviceID

Identifier of the auxiliary output device to be queried.


### -param pdwVolume

Pointer to a variable to be filled with the current volume setting. The low-order word of this location contains the left channel volume setting, and the high-order word contains the right channel setting. A value of 0xFFFF represents full volume, and a value of 0x0000 is silence.

If a device does not support both left and right volume control, the low-order word of the specified location contains the volume level.

The full 16-bit setting(s) set with the <a href="https://msdn.microsoft.com/886acacd-f2ac-4e75-aa3d-668e6d4fbbf2">auxSetVolume</a> function are returned, regardless of whether the device supports the full 16 bits of volume-level control.


## -returns



Returns MMSYSERR_NOERROR if successful or an error otherwise. Possible error values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_BADDEVICEID</b></dt>
</dl>
</td>
<td width="60%">
Specified device identifier is out of range.

</td>
</tr>
</table>
 




## -remarks



Not all devices support volume control. To determine whether a device supports volume control, use the AUXCAPS_VOLUME flag to test the <b>dwSupport</b> member of the <a href="https://msdn.microsoft.com/5b94a468-88b2-40a4-b28d-49f262e62749">AUXCAPS</a> structure (filled by the <a href="https://msdn.microsoft.com/c0920425-fb42-4112-b0c1-f4b607b9e794">auxGetDevCaps</a> function).

To determine whether a device supports volume control on both the left and right channels, use the AUXCAPS_LRVOLUME flag to test the <b>dwSupport</b> member of the <a href="https://msdn.microsoft.com/5b94a468-88b2-40a4-b28d-49f262e62749">AUXCAPS</a> structure (filled by <a href="https://msdn.microsoft.com/c0920425-fb42-4112-b0c1-f4b607b9e794">auxGetDevCaps</a>).




## -see-also




<a href="https://msdn.microsoft.com/3188355c-65be-4372-8e87-e7f755982592">Waveform Audio</a>



<a href="https://msdn.microsoft.com/6c8aaa54-0477-484f-91e1-d2152aa9c185">Waveform Functions</a>
 

 
