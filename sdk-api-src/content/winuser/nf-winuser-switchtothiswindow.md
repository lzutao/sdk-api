---
UID: NF:winuser.SwitchToThisWindow
title: SwitchToThisWindow function
author: windows-sdk-content
description: Switches focus to the specified window and brings it to the foreground.
old-location: winmsg\switchtothiswindow.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\windows\windowreference\windowfunctions\switchtothiswindow.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SwitchToThisWindow, SwitchToThisWindow function [Windows and Messages], _win32_SwitchToThisWindow, _win32_switchtothiswindow_cpp, winmsg.switchtothiswindow, winui._win32_switchtothiswindow, winuser/SwitchToThisWindow
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
 - Ext-MS-Win-NTUser-Window-L1-1-4.dll
api_name:
 - SwitchToThisWindow
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SwitchToThisWindow function


## -description


<p class="CCE_Message">[This function is not intended for general
      use. It may
      be altered or unavailable in subsequent versions of Windows.]

Switches
		 focus to the specified window and brings it to the foreground.


## -parameters




### -param hwnd [in]

Type: <b>HWND</b>

A handle to the window. 


### -param fUnknown [in]

Type: <b>BOOL</b>

A <b>TRUE</b> for this parameter indicates that the window
				is being switched to using the Alt/Ctl+Tab key sequence.  This parameter
				should be <b>FALSE</b> otherwise. 


## -returns



This function does not return a value.




## -remarks



This function is typically called to maintain window z-ordering. 

This function was not included in the SDK headers and libraries until Windows XP with Service Pack 1 (SP1) and Windows Server 2003. If you do not have a header file and import library for this function, you can call the function using <a href="https://msdn.microsoft.com/d936b4dd-058c-48e1-834b-b47ef6d8ef65">LoadLibrary</a> and <a href="https://msdn.microsoft.com/a0d7fc09-f888-4f46-a571-d3719a627597">GetProcAddress</a>.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms633530(v=VS.85).aspx">IsWindowVisible</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms633548(v=VS.85).aspx">ShowWindow</a>



<a href="https://msdn.microsoft.com/en-us/library/ms632595(v=VS.85).aspx">Windows</a>
 

 
