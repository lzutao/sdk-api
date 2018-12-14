---
UID: NF:commctrl.Edit_SetCaretIndex
title: Edit_SetCaretIndex macro
author: windows-sdk-content
description: Sets the character index at which to locate the caret. You can use this macro or send the EM_SETCARETINDEX message explicitly.
old-location: controls\edit_setcaretindex.htm
tech.root: controls
ms.assetid: 62D60717-4FE6-4738-8504-791CDE7C15E3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Edit_SetCaretIndex, Edit_SetCaretIndex macro [Windows Controls], commctrl/Edit_SetCaretIndex, controls.edit_setcaretindex
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: macro
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1809 [desktop apps only]
req.target-min-winversvr: Windows Server [desktop apps only]
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
 - Commctrl.h
api_name:
 - Edit_SetCaretIndex
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# Edit_SetCaretIndex macro


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

Sets the character index at which to locate the caret. You can use this macro or send the <a href="https://msdn.microsoft.com/8B67AD8C-A94E-49E8-98DF-EDF811270A75">EM_SETCARETINDEX</a> message explicitly.


## -parameters




### -param hwndCtl

A handle to the edit control.


### -param newCaretPosition

The character index.
