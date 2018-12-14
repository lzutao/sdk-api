---
UID: NF:shlobj_core.IShellFolderView.Select
title: IShellFolderView::Select
author: windows-sdk-content
description: IShellFolderView::Select may be altered or unavailable.
old-location: shell\IShellFolderView_Select.htm
tech.root: shell
ms.assetid: 80ec6587-515f-4697-8a19-8c486bec3473
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IShellFolderView interface [Windows Shell],Select method, IShellFolderView.Select, IShellFolderView::Select, SFVS_SELECT_ALLITEMS, SFVS_SELECT_INVERT, SFVS_SELECT_NONE, Select, Select method [Windows Shell], Select method [Windows Shell],IShellFolderView interface, _shell_IShellFolderView_Select, shell.IShellFolderView_Select, shlobj_core/IShellFolderView::Select
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
 - Shlobj_core.h
api_name:
 - IShellFolderView.Select
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IShellFolderView::Select


## -description


<p class="CCE_Message">[<b>IShellFolderView::Select</b> is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions.]

Selects and unselects items in the view.


## -parameters




### -param dwFlags

Type: <b>UINT</b>

Determines which items in the view are selected, if any. One of the following values.





#### SFVS_SELECT_NONE (0x0)

Unselects all of the items in the view.



#### SFVS_SELECT_ALLITEMS (0x1)

Selects all of the items in the view.



#### SFVS_SELECT_INVERT (0x2)

Selects all unselected items and unselects all selected items.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


