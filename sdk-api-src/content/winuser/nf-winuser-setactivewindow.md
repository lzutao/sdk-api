---
UID: NF:winuser.SetActiveWindow
title: SetActiveWindow function
author: windows-sdk-content
description: Activates a window. The window must be attached to the calling thread's message queue.
old-location: inputdev\setactivewindow.htm
tech.root: inputdev
ms.assetid: VS|winui|~\winui\windowsuserinterface\userinput\keyboardinput\keyboardinputreference\keyboardinputfunctions\setactivewindow.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SetActiveWindow, SetActiveWindow function [Keyboard and Mouse Input], _win32_SetActiveWindow, _win32_setactivewindow_cpp, inputdev.setactivewindow, winui._win32_setactivewindow, winuser/SetActiveWindow
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
 - API-MS-Win-NTUser-IE-Window-l1-1-0.dll
 - ie_shims.dll
 - API-MS-Win-RTCore-NTUser-Window-l1-1-0.dll
 - minuser.dll
 - Ext-MS-Win-RTCore-NTUser-Window-Ext-l1-1-0.dll
 - Ext-MS-Win-NTUser-Window-L1-1-4.dll
api_name:
 - SetActiveWindow
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# SetActiveWindow function


## -description


Activates a window. The window must be attached to the calling thread's message queue.


## -parameters




### -param hWnd [in]

Type: <b>HWND</b>

A handle to the top-level window to be activated.


## -returns



Type: <b>HWND</b>

If the function succeeds, the return value is the handle to the window that was previously active.

If the function fails, the return value is <b>NULL</b>. To get extended error information, call <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.




## -remarks



The <b>SetActiveWindow</b> function activates a window, but not if the application is in the background. The window will be brought into the foreground (top of <a href="https://msdn.microsoft.com/en-us/library/ms632599(v=VS.85).aspx">Z-Order</a>) if its application is in the foreground when the system activates the window.

If the window identified by the 
    <i>hWnd</i> parameter was created by the calling thread, the active window status of the calling thread is set to 
    <i>hWnd</i>. Otherwise, the active window status of the calling thread is set to <b>NULL</b>.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms646292(v=VS.85).aspx">GetActiveWindow</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645530(v=VS.85).aspx">Keyboard Input</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms633539(v=VS.85).aspx">SetForegroundWindow</a>



<a href="https://msdn.microsoft.com/en-us/library/ms646274(v=VS.85).aspx">WM_ACTIVATE</a>
 

 
