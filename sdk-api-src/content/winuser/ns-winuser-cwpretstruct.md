---
UID: NS:winuser.tagCWPRETSTRUCT
title: CWPRETSTRUCT
author: windows-sdk-content
description: Defines the message parameters passed to a WH_CALLWNDPROCRET hook procedure, CallWndRetProc.
old-location: winmsg\cwpretstruct.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\hooks\hookreference\hookstructures\cwpretstruct.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPCWPRETSTRUCT, *NPCWPRETSTRUCT, *PCWPRETSTRUCT, CWPRETSTRUCT, CWPRETSTRUCT structure [Windows and Messages], LPCWPRETSTRUCT, LPCWPRETSTRUCT structure pointer [Windows and Messages], PCWPRETSTRUCT, PCWPRETSTRUCT structure pointer [Windows and Messages], _win32_CWPRETSTRUCT_str, _win32_cwpretstruct_str_cpp, winmsg.cwpretstruct, winui._win32_cwpretstruct_str, winuser/CWPRETSTRUCT, winuser/LPCWPRETSTRUCT, winuser/PCWPRETSTRUCT"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Winuser.h
api_name:
 - CWPRETSTRUCT
product: Windows
targetos: Windows
req.typenames: CWPRETSTRUCT, *PCWPRETSTRUCT, *NPCWPRETSTRUCT, *LPCWPRETSTRUCT
req.redist: 
---

# CWPRETSTRUCT structure


## -description


Defines the message parameters passed to a <b>WH_CALLWNDPROCRET</b> hook procedure, <a href="https://msdn.microsoft.com/en-us/library/ms644976(v=VS.85).aspx">CallWndRetProc</a>. 


## -struct-fields




### -field lResult

Type: <b>LRESULT</b>

The return value of the window procedure that processed the message specified by the 
					<b>message</b> value. 


### -field lParam

Type: <b>LPARAM</b>

Additional information about the message. The exact meaning depends on the 
					<b>message</b> value. 


### -field wParam

Type: <b>WPARAM</b>

Additional information about the message. The exact meaning depends on the 
					<b>message</b> value. 


### -field message

Type: <b>UINT</b>

The message. 


### -field hwnd

Type: <b>HWND</b>

A handle to the window that processed the message specified by the 
					<b>message</b> value. 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms644976(v=VS.85).aspx">CallWndRetProc</a>



<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms632589(v=VS.85).aspx">Hooks</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms644990(v=VS.85).aspx">SetWindowsHookEx</a>
 

 
