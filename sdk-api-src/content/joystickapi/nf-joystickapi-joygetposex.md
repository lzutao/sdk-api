---
UID: NF:joystickapi.joyGetPosEx
title: joyGetPosEx function
author: windows-sdk-content
description: The joyGetPosEx function queries a joystick for its position and button status.
old-location: multimedia\joygetposex.htm
tech.root: Multimedia
ms.assetid: 7376b55c-54c0-4f58-a7f9-1cb89a8db9ee
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "_win32_joyGetPosEx, joyGetPosEx, joyGetPosEx function [Windows Multimedia], joystickapi/joyGetPosEx, multimedia.joygetposex"
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
 - joyGetPosEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# joyGetPosEx function


## -description



The <b>joyGetPosEx</b> function queries a joystick for its position and button status.




## -parameters




### -param uJoyID

Identifier of the joystick to be queried. Valid values for <i>uJoyID</i> range from zero (JOYSTICKID1) to 15.


### -param pji

Pointer to a <a href="https://msdn.microsoft.com/2c07b56b-a9d5-450f-96ca-0fdaf60c52a3">JOYINFOEX</a> structure that contains extended position information and button status of the joystick. You must set the <b>dwSize</b> and <b>dwFlags</b> members or <b>joyGetPosEx</b> will fail. The information returned from <b>joyGetPosEx</b> depends on the flags you specify in <b>dwFlags</b>.


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
<dt><b>MMSYSERR_INVALPARAM</b></dt>
</dl>
</td>
<td width="60%">
An invalid parameter was passed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MMSYSERR_BADDEVICEID</b></dt>
</dl>
</td>
<td width="60%">
The specified joystick identifier is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>JOYERR_UNPLUGGED</b></dt>
</dl>
</td>
<td width="60%">
The specified joystick is not connected to the system.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>JOYERR_PARMS</b></dt>
</dl>
</td>
<td width="60%">
The specified joystick identifier is invalid.

</td>
</tr>
</table>
 




## -remarks



This function provides access to extended devices such as rudder pedals, point-of-view hats, devices with a large number of buttons, and coordinate systems using up to six axes. For joystick devices that use three axes or fewer and have fewer than four buttons, use the <a href="https://msdn.microsoft.com/84f6a19b-1573-4e36-8a2b-7c79b12bf8ba">joyGetPos</a> function.




## -see-also




<a href="https://msdn.microsoft.com/29fe25c8-51ea-4dc1-9f98-1c10d23b7b2a">Joysticks</a>



<a href="https://msdn.microsoft.com/84e47ac3-b40f-48bc-8f59-cc678d7d521e">Multimedia Joystick Functions</a>
 

 
