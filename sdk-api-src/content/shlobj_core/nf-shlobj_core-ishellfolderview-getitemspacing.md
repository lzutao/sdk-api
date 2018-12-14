---
UID: NF:shlobj_core.IShellFolderView.GetItemSpacing
title: IShellFolderView::GetItemSpacing
author: windows-sdk-content
description: Gets the spacing for small and large view modes only.
old-location: shell\IShellFolderView_GetItemSpacing.htm
tech.root: shell
ms.assetid: 92450bc7-26e5-4061-90f7-eea0f0a4db09
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetItemSpacing, GetItemSpacing method [Windows Shell], GetItemSpacing method [Windows Shell],IShellFolderView interface, IShellFolderView interface [Windows Shell],GetItemSpacing method, IShellFolderView.GetItemSpacing, IShellFolderView::GetItemSpacing, _shell_IShellFolderView_GetItemSpacing, shell.IShellFolderView_GetItemSpacing, shlobj_core/IShellFolderView::GetItemSpacing
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
 - IShellFolderView.GetItemSpacing
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IShellFolderView::GetItemSpacing


## -description


<p class="CCE_Message">[This method has been deprecated. Use <a href="https://msdn.microsoft.com/6ea81c40-773f-4f53-97c1-99619e46be48">IFolderView::GetSpacing</a> instead.]

Gets the spacing for small and large view modes only.


## -parameters




### -param pSpacing [out]

Type: <b><a href="https://msdn.microsoft.com/fcd7f3da-6aba-4683-bd5e-14a6b5f93cb5">ITEMSPACING</a>*</b>

A pointer to a structure that, when this method returns successfully, receives the information that describes the view mode spacing.


## -returns



Type: <b>HRESULT</b>

Returns <b>S_OK</b> if the current view mode is positionable; otherwise, <b>S_FALSE</b>.




## -remarks



This method sends an <a href="https://msdn.microsoft.com/en-us/library/Bb761051(v=VS.85).aspx">LVM_GETITEMSPACING</a> message to get the view mode spacing.

This method retrieves mode spacing for only the large and small view modes.

In Windows Vista and later, this method stores the small view mode spacing in both pairs of values returned in the <a href="https://msdn.microsoft.com/fcd7f3da-6aba-4683-bd5e-14a6b5f93cb5">ITEMSPACING</a> structure.


