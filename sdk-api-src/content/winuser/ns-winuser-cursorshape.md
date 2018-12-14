---
UID: NS:winuser.tagCURSORSHAPE
title: CURSORSHAPE
author: windows-sdk-content
description: Contains information about a cursor.
old-location: menurc\cursorshape.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\introductiontoresources\resourcereference\resourcestructures\cursorshape.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPCURSORSHAPE, CURSORSHAPE, CURSORSHAPE structure [Menus and Other Resources], LPCURSORSHAPE, LPCURSORSHAPE structure pointer [Menus and Other Resources], _win32_CURSORSHAPE_str, _win32_cursorshape_str_cpp, menurc.cursorshape, winui._win32_cursorshape_str, winuser/CURSORSHAPE, winuser/LPCURSORSHAPE"
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
 - CURSORSHAPE
product: Windows
targetos: Windows
req.typenames: CURSORSHAPE, *LPCURSORSHAPE
req.redist: 
---

# CURSORSHAPE structure


## -description


Contains information about a cursor.


## -struct-fields




### -field xHotSpot

Type: <b>int</b>

The horizontal position of the hot spot, relative to the upper-left corner of the cursor bitmap. 


### -field yHotSpot

Type: <b>int</b>

The vertical position of the hot spot, relative to the upper-left corner of the cursor bitmap. 


### -field cx

Type: <b>int</b>

The width, in pixels, of the cursor. 


### -field cy

Type: <b>int</b>

The height, in pixels, of the cursor. 


### -field cbWidth

Type: <b>int</b>

The width, in bytes, of the cursor bitmap. 


### -field Planes

Type: <b>BYTE</b>

The number of color planes. 


### -field BitsPixel

Type: <b>BYTE</b>

The number of bits used to indicate the color of a single pixel in the cursor. 


## -remarks



When an application passes a cursor handle to the <a href="https://msdn.microsoft.com/en-us/library/ms648047(v=VS.85).aspx">LockResource</a>function, the function returns a pointer to a buffer containing information about the cursor. An application can use the <b>CURSORSHAPE</b> structure to access the information.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms648047(v=VS.85).aspx">LockResource</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/ms632583(v=VS.85).aspx">Resources</a>
 

 
