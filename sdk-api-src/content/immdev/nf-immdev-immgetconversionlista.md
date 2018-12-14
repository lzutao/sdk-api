---
UID: NF:immdev.ImmGetConversionListA
title: ImmGetConversionListA function
author: windows-sdk-content
description: Retrieves the conversion result list of characters or words without generating any IME-related messages.
old-location: intl\immgetconversionlist.htm
tech.root: Intl
ms.assetid: c38547fa-b9d8-41a0-8d73-21056212b775
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GCL_CONVERSION, GCL_REVERSECONVERSION, GCL_REVERSE_LENGTH, ImmGetConversionList, ImmGetConversionList function [Internationalization for Windows Applications], ImmGetConversionListA, ImmGetConversionListW, _win32_ImmGetConversionList, imm/ImmGetConversionList, imm/ImmGetConversionListA, imm/ImmGetConversionListW, intl.immgetconversionlist
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: immdev.h
req.include-header: Immdev.h, Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only],East Asian language support installed.
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: ImmGetConversionListW (Unicode) and ImmGetConversionListA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Imm32.lib
req.dll: Imm32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Imm32.dll
api_name:
 - ImmGetConversionList
 - ImmGetConversionListA
 - ImmGetConversionListW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ImmGetConversionListA function


## -description


Retrieves the conversion result list of characters or words without generating any IME-related messages.


## -parameters




### -param HKL [in]

Input locale identifier.


### -param HIMC [in]

Handle to the input context.


### -param lpSrc [in]

Pointer to a null-terminated character string specifying the source of the list.


### -param lpDst [out]

Pointer to a <a href="https://msdn.microsoft.com/d60b28fb-0cdd-43b4-8d99-cb829bea6679">CANDIDATELIST</a> structure in which the function retrieves the list.


### -param dwBufLen [in]

Size, in bytes, of the output buffer. The application sets this parameter to 0 if the function is to return the buffer size required for the complete conversion result list.


### -param uFlag [in]

Action flag. This parameter can have one of the following values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="GCL_CONVERSION"></a><a id="gcl_conversion"></a><dl>
<dt><b>GCL_CONVERSION</b></dt>
</dl>
</td>
<td width="60%">
Source string is the reading string. The function copies the result string to the destination buffer.

</td>
</tr>
<tr>
<td width="40%"><a id="GCL_REVERSECONVERSION"></a><a id="gcl_reverseconversion"></a><dl>
<dt><b>GCL_REVERSECONVERSION</b></dt>
</dl>
</td>
<td width="60%">
Source string is the result string. The function copies the reading string to the destination buffer.

</td>
</tr>
<tr>
<td width="40%"><a id="GCL_REVERSE_LENGTH"></a><a id="gcl_reverse_length"></a><dl>
<dt><b>GCL_REVERSE_LENGTH</b></dt>
</dl>
</td>
<td width="60%">
Source string is the result string. The function returns the size, in bytes, of the reading string created if GCL_REVERSECONVERSION is specified.

</td>
</tr>
</table>
 


## -returns



Returns the number of bytes copied to the output buffer. If the application sets the <i>dwBufLen</i> parameter to 0, the function returns the size, in bytes, of the required output buffer.




## -see-also




<a href="https://msdn.microsoft.com/d60b28fb-0cdd-43b4-8d99-cb829bea6679">CANDIDATELIST</a>



<a href="https://msdn.microsoft.com/3e23e004-514a-4021-bd20-5ac55547258f">Input Method Manager</a>



<a href="https://msdn.microsoft.com/833c07eb-0ecf-41e2-9e01-8d83e51ffcef">Input Method Manager Functions</a>
 

 
