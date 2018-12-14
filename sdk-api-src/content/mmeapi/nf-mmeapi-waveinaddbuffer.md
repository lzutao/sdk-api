---
UID: NF:mmeapi.waveInAddBuffer
title: waveInAddBuffer function
author: windows-sdk-content
description: The waveInAddBuffer function sends an input buffer to the given waveform-audio input device. When the buffer is filled, the application is notified.
old-location: multimedia\waveinaddbuffer.htm
tech.root: Multimedia
ms.assetid: 343abdb6-7a0f-4756-9920-60d308e845f9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "_win32_waveInAddBuffer, mmeapi/waveInAddBuffer, multimedia.waveinaddbuffer, waveInAddBuffer, waveInAddBuffer function [Windows Multimedia]"
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
 - waveInAddBuffer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# waveInAddBuffer function


## -description



The <b>waveInAddBuffer</b> function sends an input buffer to the given waveform-audio input device. When the buffer is filled, the application is notified.




## -parameters




### -param hwi

Handle to the waveform-audio input device.


### -param pwh

Pointer to a <a href="https://msdn.microsoft.com/be70ae8e-8d8f-4261-bd0e-c6fd7feec520">WAVEHDR</a> structure that identifies the buffer.


### -param cbwh

Size, in bytes, of the <b>WAVEHDR</b> structure.


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
<dt><b>MMSYSERR_INVALHANDLE</b></dt>
</dl>
</td>
<td width="60%">
Specified device handle is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_NODRIVER</b></dt>
</dl>
</td>
<td width="60%">
No device driver is present.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_NOMEM</b></dt>
</dl>
</td>
<td width="60%">
Unable to allocate or lock memory.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WAVERR_UNPREPARED</b></dt>
</dl>
</td>
<td width="60%">
The buffer pointed to by the <i>pwh</i> parameter hasn't been prepared.

</td>
</tr>
</table>
 




## -remarks



When the buffer is filled, the WHDR_DONE bit is set in the <b>dwFlags</b> member of the <b>WAVEHDR</b> structure.

The buffer must be prepared with the <b>waveInPrepareHeader</b> function before it is passed to this function.




## -see-also




<a href="https://msdn.microsoft.com/3188355c-65be-4372-8e87-e7f755982592">Waveform Audio</a>



<a href="https://msdn.microsoft.com/6c8aaa54-0477-484f-91e1-d2152aa9c185">Waveform Functions</a>
 

 
