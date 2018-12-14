---
UID: NF:winuser.EnableWindow
title: EnableWindow function
author: windows-sdk-content
description: Enables or disables mouse and keyboard input to the specified window or control. When input is disabled, the window does not receive input such as mouse clicks and key presses. When input is enabled, the window receives all input.
old-location: inputdev\enablewindow.htm
tech.root: inputdev
ms.assetid: VS|winui|~\winui\windowsuserinterface\userinput\keyboardinput\keyboardinputreference\keyboardinputfunctions\enablewindow.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EnableWindow, EnableWindow function [Keyboard and Mouse Input], _win32_EnableWindow, _win32_enablewindow_cpp, inputdev.enablewindow, winui._win32_enablewindow, winuser/EnableWindow
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
 - Ext-MS-Win-NTUser-Keyboard-l1-1-0.dll
 - Ext-MS-Win-NTUser-Keyboard-l1-1-1.dll
 - Ext-MS-Win-RTCore-NTUser-Window-Ext-l1-1-0.dll
 - ext-ms-win-ntuser-keyboard-l1-1-2.dll
 - Ext-MS-Win-NTUser-Keyboard-L1-2-0.dll
 - Ext-MS-Win-NTUser-Keyboard-L1-2-1.dll
 - Ext-MS-Win-NTUser-Window-L1-1-4.dll
api_name:
 - EnableWindow
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# EnableWindow function


## -description


Enables or disables mouse and keyboard input to the specified window or control. When input is disabled, the window does not receive input such as mouse clicks and key presses. When input is enabled, the window receives all input.


## -parameters




### -param hWnd [in]

Type: <b>HWND</b>

A handle to the window to be enabled or disabled.


### -param bEnable [in]

Type: <b>BOOL</b>

Indicates whether to enable or disable the window. If this parameter is <b>TRUE</b>, the window is enabled. If the parameter is <b>FALSE</b>, the window is disabled.


## -returns



Type: <b>BOOL</b>

If the window was previously disabled, the return value is nonzero.

If the window was not previously disabled, the return value is zero.




## -remarks



If the window is being disabled, the system sends a <a href="https://msdn.microsoft.com/en-us/library/ms632615(v=VS.85).aspx">WM_CANCELMODE</a> message. If the enabled state of a window is changing, the system sends a <a href="https://msdn.microsoft.com/en-us/library/ms632621(v=VS.85).aspx">WM_ENABLE</a> message after the <b>WM_CANCELMODE</b> message. (These messages are sent before <b>EnableWindow</b> returns.) If a window is already disabled, its child windows are implicitly disabled, although they are not sent a <b>WM_ENABLE</b> message.

A window must be enabled before it can be activated. For example, if an application is displaying a modeless dialog box and has disabled its main window, the application must enable the main window before destroying the dialog box. Otherwise, another window will receive the keyboard focus and be activated. If a child window is disabled, it is ignored when the system tries to determine which window should receive mouse messages.

By default, a window is enabled when it is created. To create a window that is initially disabled, an application can specify the <b>WS_DISABLED</b> style in the <a href="https://msdn.microsoft.com/en-us/library/ms632679(v=VS.85).aspx">CreateWindow</a> or <a href="https://msdn.microsoft.com/en-us/library/ms632680(v=VS.85).aspx">CreateWindowEx</a> function. After a window has been created, an application can use <b>EnableWindow</b> to enable or disable the window.

An application can use this function to enable or disable a control in a dialog box. A disabled control cannot receive the keyboard focus, nor can a user gain access to it.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms632679(v=VS.85).aspx">CreateWindow</a>



<a href="https://msdn.microsoft.com/en-us/library/ms632680(v=VS.85).aspx">CreateWindowEx</a>



<a href="https://msdn.microsoft.com/en-us/library/ms646303(v=VS.85).aspx">IsWindowEnabled</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645530(v=VS.85).aspx">Keyboard Input</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms632621(v=VS.85).aspx">WM_ENABLE</a>
 

 
