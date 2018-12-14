---
UID: NF:shlobj_core.IActiveDesktop.GetDesktopItemBySource
title: IActiveDesktop::GetDesktopItemBySource
author: windows-sdk-content
description: Gets a desktop item using its source URL.
old-location: lwef\iactivedesktop_getdesktopitembysource.htm
tech.root: lwef
ms.assetid: 9449238a-c1af-493c-9c23-503317fe6656
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDesktopItemBySource, GetDesktopItemBySource method [Legacy Windows Environment Features], GetDesktopItemBySource method [Legacy Windows Environment Features],IActiveDesktop interface, IActiveDesktop interface [Legacy Windows Environment Features],GetDesktopItemBySource method, IActiveDesktop.GetDesktopItemBySource, IActiveDesktop::GetDesktopItemBySource, _win32_IActiveDesktop_GetDesktopItemBySource, lwef.iactivedesktop_getdesktopitembysource, shell.iactivedesktop_getdesktopitembysource, shlobj_core/IActiveDesktop::GetDesktopItemBySource
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shlobj_core.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
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
req.dll: Shell32.dll (version 4.71 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Shell32.dll
api_name:
 - IActiveDesktop.GetDesktopItemBySource
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IActiveDesktop::GetDesktopItemBySource


## -description


Gets a desktop item using its source URL.


## -parameters




### -param pwszSource [in]

Type: <b>PCWSTR</b>

A pointer to a string that contains the source URL of the desktop item.


### -param pcomp [in, out]

Type: <b>LPCOMPONENT</b>

A pointer to the <a href="https://msdn.microsoft.com/2692a2d6-1d33-410f-987c-8388c636cae6">COMPONENT</a> structure that, when this method returns successfully, receives the details about the desktop item. On entry, the size of the structure must be set.


### -param dwReserved

Type: <b>DWORD</b>

Reserved. Must be set to zero. 


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/4d572b86-36e8-417b-857c-eb477c04c691">IActiveDesktop</a>
 

 
