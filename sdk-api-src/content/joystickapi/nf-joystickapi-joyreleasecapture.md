---
UID: NF:joystickapi.joyReleaseCapture
title: joyReleaseCapture function
author: windows-sdk-content
description: The joyReleaseCapture function releases the specified captured joystick.
old-location: multimedia\joyreleasecapture.htm
tech.root: Multimedia
ms.assetid: deb1f280-12bd-4e4d-841a-667b7785207c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "_win32_joyReleaseCapture, joyReleaseCapture, joyReleaseCapture function [Windows Multimedia], joystickapi/joyReleaseCapture, multimedia.joyreleasecapture"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: joystickapi.h
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
 - API-MS-Win-mm-joystick-l1-1-0.dll
 - winmmbase.dll
api_name:
 - joyReleaseCapture
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# joyReleaseCapture function


## -description



The <b>joyReleaseCapture</b> function releases the specified captured joystick.




## -parameters




### -param uJoyID

Identifier of the joystick to be released. Valid values for <i>uJoyID</i> range from zero (JOYSTICKID1) to 15.


## -returns



Returns JOYERR_NOERROR if successful or one of the following error values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_NODRIVER</b></dt>
</dl>
</td>
<td width="60%">
The joystick driver is not present.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_INVALIDPARAM</b></dt>
</dl>
</td>
<td width="60%">
The specified joystick device identifier <i>uJoyID</i> is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>JOYERR_PARMS</b></dt>
</dl>
</td>
<td width="60%">
The specified joystick device identifier <i>uJoyID</i> is invalid.

</td>
</tr>
</table>
 




## -remarks



This method returns JOYERR_NOERROR when passed a valid joystick identifier that has not been captured.




## -see-also




<a href="https://msdn.microsoft.com/29fe25c8-51ea-4dc1-9f98-1c10d23b7b2a">Joysticks</a>



<a href="https://msdn.microsoft.com/84e47ac3-b40f-48bc-8f59-cc678d7d521e">Multimedia Joystick Functions</a>
 

 
