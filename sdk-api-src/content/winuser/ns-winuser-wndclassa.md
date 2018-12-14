---
UID: NS:winuser.tagWNDCLASSA
title: WNDCLASSA
author: windows-sdk-content
description: Contains the window class attributes that are registered by the RegisterClass function.
old-location: winmsg\wndclass.htm
tech.root: winmsg
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\windowclasses\windowclassreference\windowclassstructures\wndclass.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPWNDCLASSA, *NPWNDCLASSA, *PWNDCLASSA, PWNDCLASS, PWNDCLASS structure pointer [Windows and Messages], WNDCLASS, WNDCLASS structure [Windows and Messages], WNDCLASSA, WNDCLASSW, _win32_WNDCLASS_str, _win32_wndclass_str_cpp, winmsg.wndclass, winui._win32_wndclass_str, winuser/PWNDCLASS, winuser/WNDCLASS, winuser/WNDCLASSA, winuser/WNDCLASSW"
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
req.unicode-ansi: WNDCLASSW (Unicode) and WNDCLASSA (ANSI)
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
 - WNDCLASS
 - WNDCLASSA
 - WNDCLASSW
product: Windows
targetos: Windows
req.typenames: WNDCLASSA, *PWNDCLASSA, *NPWNDCLASSA, *LPWNDCLASSA
req.redist: 
---

# WNDCLASSA structure


## -description


Contains the window class attributes that are registered by the <a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a> function. 

This structure has been superseded by the <a href="https://msdn.microsoft.com/f7e60154-b52c-4dee-b6dd-b6a4882ad4a9">WNDCLASSEX</a> structure used with the <a href="https://msdn.microsoft.com/f48ba5a5-08c7-4d16-bc25-e028ea9a73f4">RegisterClassEx</a> function. You can still use <b>WNDCLASS</b> and <a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a> if you do not need to set the small icon associated with the window class.


## -struct-fields




### -field style

Type: <b>UINT</b>

The class style(s). This member can be any combination of the <a href="about_window_classes.htm">Class Styles</a>. 


### -field lpfnWndProc

Type: <b>WNDPROC</b>

A pointer to the window procedure. You must use the <a href="https://msdn.microsoft.com/667449cd-1eea-43de-8268-3da73022d7ac">CallWindowProc</a> function to call the window procedure. For more information, see <a href="https://msdn.microsoft.com/4bb1cc3d-78db-4546-8ae9-d29fc6ee8f7c">WindowProc</a>. 


### -field cbClsExtra

Type: <b>int</b>

The number of extra bytes to allocate following the window-class structure. The system initializes the bytes to zero. 


### -field cbWndExtra

Type: <b>int</b>

The number of extra bytes to allocate following the window instance. The system initializes the bytes to zero. If an application uses <b>WNDCLASS</b> to register a dialog box created by using the 
					<b>CLASS</b> directive in the resource file, it must set this member to <b>DLGWINDOWEXTRA</b>. 


### -field hInstance

Type: <b>HINSTANCE</b>

A handle to the instance that contains the window procedure for the class. 


### -field hIcon

Type: <b>HICON</b>

A handle to the class icon. This member must be a handle to an icon resource. If this member is <b>NULL</b>, the system provides a default icon. 


### -field hCursor

Type: <b>HCURSOR</b>

A handle to the class cursor. This member must be a handle to a cursor resource. If this member is <b>NULL</b>, an application must explicitly set the cursor shape whenever the mouse moves into the application's window. 


### -field hbrBackground

Type: <b>HBRUSH</b>

A handle to the class background brush. This member can be a handle to the physical brush to be used for painting the background, or it can be a color value. A color value must be one of the following standard system colors (the value 1 must be added to the chosen color). If a color value is given, you must convert it to one of the following 
<b>HBRUSH</b> types: 


<ul>
<li>COLOR_ACTIVEBORDER</li>
<li>COLOR_ACTIVECAPTION</li>
<li>COLOR_APPWORKSPACE</li>
<li>COLOR_BACKGROUND</li>
<li>COLOR_BTNFACE</li>
<li>COLOR_BTNSHADOW</li>
<li>COLOR_BTNTEXT</li>
<li>COLOR_CAPTIONTEXT</li>
<li>COLOR_GRAYTEXT</li>
<li>COLOR_HIGHLIGHT</li>
<li>COLOR_HIGHLIGHTTEXT</li>
<li>COLOR_INACTIVEBORDER</li>
<li>COLOR_INACTIVECAPTION</li>
<li>COLOR_MENU</li>
<li>COLOR_MENUTEXT</li>
<li>COLOR_SCROLLBAR</li>
<li>COLOR_WINDOW</li>
<li>COLOR_WINDOWFRAME</li>
<li>COLOR_WINDOWTEXT </li>
</ul>
The system automatically deletes class background brushes when the class is unregistered by using <a href="https://msdn.microsoft.com/ce0277a9-082e-49ef-b8fd-779284303ffa">UnregisterClass</a>. An application should not delete these brushes. 

When this member is <b>NULL</b>, an application must paint its own background whenever it is requested to paint in its client area. To determine whether the background must be painted, an application can either process the 
						<a href="https://msdn.microsoft.com/3bdc37da-227c-4be1-bf0b-99704b8acbe1">WM_ERASEBKGND</a> message or test the 
						<b>fErase</b> member of the <a href="https://msdn.microsoft.com/1f8c6dd2-e511-48f2-8ab0-d2fadb1ce433">PAINTSTRUCT</a> structure filled by the <a href="https://msdn.microsoft.com/513341d7-bed8-469c-a067-ee71dc8860f9">BeginPaint</a> function. 


### -field lpszMenuName

Type: <b>LPCTSTR</b>

The resource name of the class menu, as the name appears in the resource file. If you use an integer to identify the menu, use the <a href="https://msdn.microsoft.com/761df981-776f-43ca-9cc9-bb82a49f66e6">MAKEINTRESOURCE</a> macro. If this member is <b>NULL</b>, windows belonging to this class have no default menu. 


### -field lpszClassName

Type: <b>LPCTSTR</b>

A pointer to a null-terminated string or is an atom. If this parameter is an atom, it must be a class atom created by a previous call to the <a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a> or <a href="https://msdn.microsoft.com/f48ba5a5-08c7-4d16-bc25-e028ea9a73f4">RegisterClassEx</a> function. The atom must be in the low-order word of 
					<b>lpszClassName</b>; the high-order word must be zero. 
					

If <b>lpszClassName</b> is a string, it specifies the window class name. The class name can be any name registered with <a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a> or <a href="https://msdn.microsoft.com/f48ba5a5-08c7-4d16-bc25-e028ea9a73f4">RegisterClassEx</a>, or any of the predefined control-class names. 

The maximum length for <b>lpszClassName</b> is 256. If <b>lpszClassName</b> is greater than the maximum length, the <a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a> function will fail.


## -see-also




<a href="https://msdn.microsoft.com/513341d7-bed8-469c-a067-ee71dc8860f9">BeginPaint</a>



<b>Conceptual</b>



<a href="https://msdn.microsoft.com/5424b87c-22ea-414e-840e-214d9f0dc9ad">CreateWindow</a>



<a href="https://msdn.microsoft.com/33deeb92-6285-4c67-9338-ca2e194b9915">CreateWindowEx</a>



<a href="https://msdn.microsoft.com/50b2387b-c8e4-42a8-8f0f-0bdb355adbfd">GetDC</a>



<a href="https://msdn.microsoft.com/761df981-776f-43ca-9cc9-bb82a49f66e6">MAKEINTRESOURCE</a>



<b>Other Resources</b>



<a href="https://msdn.microsoft.com/1f8c6dd2-e511-48f2-8ab0-d2fadb1ce433">PAINTSTRUCT</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/485115e5-b4ec-4e93-89ce-eee229ccabb7">RegisterClass</a>



<a href="https://msdn.microsoft.com/ce0277a9-082e-49ef-b8fd-779284303ffa">UnregisterClass</a>



<a href="https://msdn.microsoft.com/afebaa07-cf00-47db-a919-46436f164881">WM_PAINT</a>



<a href="https://msdn.microsoft.com/f7e60154-b52c-4dee-b6dd-b6a4882ad4a9">WNDCLASSEX</a>



<a href="https://msdn.microsoft.com/6ef633db-af76-42d6-b211-96846578eaac">Window Classes</a>



<a href="https://msdn.microsoft.com/4bb1cc3d-78db-4546-8ae9-d29fc6ee8f7c">WindowProc</a>
 

 
