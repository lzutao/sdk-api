---
UID: NF:shlobj_core.IShellFolderView.GetDropPoint
title: IShellFolderView::GetDropPoint
author: windows-sdk-content
description: Gets the point at which the current drag-and-drop operation was terminated.
old-location: shell\IShellFolderView_GetDropPoint.htm
tech.root: shell
ms.assetid: 2ea09e0f-adf0-4d33-a7c7-c8a4aa6b30ea
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDropPoint, GetDropPoint method [Windows Shell], GetDropPoint method [Windows Shell],IShellFolderView interface, IShellFolderView interface [Windows Shell],GetDropPoint method, IShellFolderView.GetDropPoint, IShellFolderView::GetDropPoint, _shell_IShellFolderView_GetDropPoint, shell.IShellFolderView_GetDropPoint, shlobj_core/IShellFolderView::GetDropPoint
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shlobj_core.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - COM
api_location:
 - shlobj_core.h
api_name:
 - IShellFolderView.GetDropPoint
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IShellFolderView::GetDropPoint


## -description


<p class="CCE_Message">[This method is available through Windows Vista. It might be altered or unavailable in subsequent versions of Windows.]

Gets the point at which the current drag-and-drop operation was terminated.


## -parameters




### -param ppt [out]

Type: <b><a href="https://msdn.microsoft.com/ecb0f0e1-90c2-48ab-a069-552262b49c7c">POINT</a>*</b>

A pointer to a structure that, when this method returns successfully, receives the coordinates at which the current drag-and-drop operation was terminated.


## -returns



Type: <b>HRESULT</b>

Returns<b> S_OK</b> if successful, <b>S_FALSE</b> if the view does not have a drop point, or an error value otherwise.


