---
UID: NF:utilapiset.Beep
title: Beep function
author: windows-sdk-content
description: Generates simple tones on the speaker.
old-location: base\beep.htm
tech.root: debug
ms.assetid: ea74fe2a-759e-4466-bef4-6061643ddd26
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Beep, Beep function, _win32_beep, base.beep, utilapiset/Beep
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: utilapiset.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
 - API-MS-Win-Core-util-l1-1-0.dll
 - KernelBase.dll
 - MinKernelBase.dll
 - api-ms-win-downlevel-kernel32-l1-1-0.dll
 - api-ms-win-core-util-l1-1-1.dll
api_name:
 - Beep
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# Beep function


## -description


Generates simple tones on the speaker. The function is synchronous; it performs an alertable wait and does not return control to its caller until the sound finishes.


## -parameters




### -param dwFreq [in]

The frequency of the sound, in hertz. This parameter must be in the range 37 through 32,767 (0x25 through 0x7FFF). 



					


### -param dwDuration [in]

The duration of the sound, in milliseconds. 



					


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call 
<a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



 A long time ago, all PC computers shared a common 8254 programable interval timer chip for the generation of primitive sounds.  The <b>Beep</b> function was written specifically to emit a beep on that piece of hardware.  

On these older systems, muting and volume controls have no effect on <b>Beep</b>; you would still hear the tone. To silence the tone, you used the following commands:

<b>net stop beep</b>

<b>sc config beep start= disabled</b>

Since then, sound cards have become standard equipment on almost all PC computers.  As sound cards became more common, manufacturers began to remove the old timer chip from computers.   The chips were also excluded from the design of server computers.  The result is that <b>Beep</b> did not work on all computers without the chip.  This was okay because most developers had moved on to calling the <a href="https://msdn.microsoft.com/70681472-36a5-4ae3-b769-0421cf97ff2a">MessageBeep</a> function that uses whatever is the default sound device instead of the 8254 chip.  

Eventually because of the lack of hardware to communicate with, support for <b>Beep</b> was dropped in Windows Vista and Windows XP 64-Bit Edition.

In Windows 7,  <b>Beep</b> was rewritten to pass the beep to the default sound device for the session.  This is normally the sound card, except when run under Terminal Services, in which case the beep is rendered on the client.


#### Examples

The following example demonstrates the use of this function.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>Beep( 750, 300 );
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/ae8ad3a2-1f1a-46d6-adaa-74c50c07dcc5">Error Handling Functions</a>



<a href="https://msdn.microsoft.com/70681472-36a5-4ae3-b769-0421cf97ff2a">MessageBeep</a>



<a href="https://msdn.microsoft.com/35b6e93c-323a-4592-9394-a2e9dd79d9e6">Notifying the User</a>
 

 
