---
UID: NS:joystickapi.joyinfo_tag
title: JOYINFO
author: windows-sdk-content
description: The JOYINFO structure contains information about the joystick position and button state.
old-location: multimedia\joyinfo.htm
tech.root: Multimedia
ms.assetid: 9f21fdcc-6940-44de-8adf-28190c0cc7c0
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPJOYINFO, *NPJOYINFO, *PJOYINFO, JOYINFO, JOYINFO structure [Windows Multimedia], _win32_JOYINFO_str, joyinfo_tag, joystickapi/JOYINFO, multimedia.joyinfo"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - joystickapi.h
api_name:
 - JOYINFO
product: Windows
targetos: Windows
req.typenames: JOYINFO, *PJOYINFO, *NPJOYINFO, *LPJOYINFO
req.redist: 
---

# JOYINFO structure


## -description



The <b>JOYINFO</b> structure contains information about the joystick position and button state.




## -struct-fields




### -field wXpos

Current X-coordinate.


### -field wYpos

Current Y-coordinate.


### -field wZpos

Current Z-coordinate.


### -field wButtons

Current state of joystick buttons described by one or more of the following values:

<table>
<tr>
<th>Button</th>
<th>Description</th>
</tr>
<tr>
<td>JOY_BUTTON1</td>
<td>First joystick button is pressed.</td>
</tr>
<tr>
<td>JOY_BUTTON2</td>
<td>Second joystick button is pressed.</td>
</tr>
<tr>
<td>JOY_BUTTON3</td>
<td>Third joystick button is pressed.</td>
</tr>
<tr>
<td>JOY_BUTTON4</td>
<td>Fourth joystick button is pressed.</td>
</tr>
</table>
 


## -see-also




Joysticks



Multimedia Joystick Structures
 

 
