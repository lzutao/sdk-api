---
UID: NF:winuser.InternalGetWindowText
title: InternalGetWindowText function
author: windows-sdk-content
description: Copies the text of the specified window's title bar (if it has one) into a buffer.
old-location: winmsg\internalgetwindowtext.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\windows\windowreference\windowfunctions\internalgetwindowtext.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: InternalGetWindowText, InternalGetWindowText function [Windows and Messages], _win32_InternalGetWindowText, _win32_internalgetwindowtext_cpp, winmsg.internalgetwindowtext, winui._win32_internalgetwindowtext, winuser/InternalGetWindowText
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winuser.h
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
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - User32.dll
api_name:
 - InternalGetWindowText
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# InternalGetWindowText function


## -description


<p class="CCE_Message">[This function is not intended for general
      use. It may
      be altered or unavailable in subsequent versions of Windows.]

Copies the text of the specified window's title bar (if it has one) into a buffer.

This function is similar to the <a href="https://msdn.microsoft.com/en-us/library/ms633520(v=VS.85).aspx">GetWindowText</a> function.
		However, it obtains the window text directly from the window structure
		associated with the specified window's handle and then always provides the text as a
		Unicode string. This is unlike <b>GetWindowText</b> which obtains the
		text by sending the window a <a href="https://msdn.microsoft.com/en-us/library/ms632627(v=VS.85).aspx">WM_GETTEXT</a> message.  If the
		specified window is a control, the text of the control is obtained. 


## -parameters




### -param hWnd [in]

Type: <b>HWND</b>

A handle to the window or control containing the text. 


### -param pString [out]

Type: <b>LPWSTR</b>

The buffer that is to receive the text.
				
				If the
				string is as long or longer than the buffer, the string is truncated and
				terminated with a null character. 


### -param cchMaxCount [in]

Type: <b>int</b>

The maximum number of characters to be copied to the buffer,
				including the null character. If the text exceeds this limit,
				it is truncated. 


## -returns



Type: <strong>Type: <b>int</b>
</strong>

If the function succeeds, the return value is the length, in characters,
				of the copied string, not including the terminating null character.
				If the window has no title bar or text, if the title bar is empty, or if the window
				or control handle is invalid, the return value is zero. To get extended error
				information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>. 




## -remarks



This function was not included in the SDK headers and libraries until Windows XP with Service Pack 1 (SP1) and Windows Server 2003. If you do not have a header file and import library for this function, you can call the function using <a href="https://msdn.microsoft.com/d936b4dd-058c-48e1-834b-b47ef6d8ef65">LoadLibrary</a> and <a href="https://msdn.microsoft.com/a0d7fc09-f888-4f46-a571-d3719a627597">GetProcAddress</a>.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms633520(v=VS.85).aspx">GetWindowText</a>



<a href="https://msdn.microsoft.com/en-us/library/ms633521(v=VS.85).aspx">GetWindowTextLength</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms633546(v=VS.85).aspx">SetWindowText</a>



<a href="https://msdn.microsoft.com/en-us/library/ms644928(v=VS.85).aspx">Using Messages and Message Queues</a>



<a href="https://msdn.microsoft.com/en-us/library/ms632627(v=VS.85).aspx">WM_GETTEXT</a>



<a href="https://msdn.microsoft.com/en-us/library/ms632595(v=VS.85).aspx">Windows</a>
 

 
