---
UID: NF:mmiscapi.mmioStringToFOURCCW
title: mmioStringToFOURCCW function
author: windows-sdk-content
description: The mmioStringToFOURCC function converts a null-terminated string to a four-character code.
old-location: multimedia\mmiostringtofourcc.htm
tech.root: Multimedia
ms.assetid: e2d4f7f0-7827-4af0-baa8-02607369247a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "_win32_mmioStringToFOURCC, mmioStringToFOURCC, mmioStringToFOURCC function [Windows Multimedia], mmioStringToFOURCCA, mmioStringToFOURCCW, mmsystem/mmioStringToFOURCC, mmsystem/mmioStringToFOURCCA, mmsystem/mmioStringToFOURCCW, multimedia.mmiostringtofourcc"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: mmiscapi.h
req.include-header: Mmiscapi.h, Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: mmioStringToFOURCCW (Unicode) and mmioStringToFOURCCA (ANSI)
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
 - API-MS-Win-mm-misc-l1-1-0.dll
 - winmmbase.dll
 - API-MS-Win-mm-misc-l1-1-1.dll
api_name:
 - mmioStringToFOURCC
 - mmioStringToFOURCCA
 - mmioStringToFOURCCW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# mmioStringToFOURCCW function


## -description



The <b>mmioStringToFOURCC</b> function converts a null-terminated string to a four-character code.




## -parameters




### -param sz

Pointer to a null-terminated string to convert to a four-character code.


### -param uFlags

Flags for the conversion. The following value is defined:

<table>
<tr>
<th>Value
</th>
<th>Meaning
</th>
</tr>
<tr>
<td>MMIO_TOUPPER</td>
<td>Converts all characters to uppercase.</td>
</tr>
</table>
 


## -returns



Returns the four-character code created from the given string.




## -remarks



This function copies the string to a four-character code and pads it with space characters or truncates it if necessary. It does not check whether the code it returns is valid.


