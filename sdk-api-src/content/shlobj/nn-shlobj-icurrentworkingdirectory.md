---
UID: NN:shlobj.ICurrentWorkingDirectory
title: ICurrentWorkingDirectory
author: windows-sdk-content
description: Exposes methods that enable a client to retrieve or set an object's current working directory.
old-location: shell\ICurrentWorkingDirectory.htm
tech.root: shell
ms.assetid: 1fdbe616-3ca3-4f07-b89c-4c76561ba169
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ICurrentWorkingDirectory, ICurrentWorkingDirectory interface [Windows Shell], ICurrentWorkingDirectory interface [Windows Shell],described, _win32_ICurrentWorkingDirectory, shell.ICurrentWorkingDirectory, shlobj/ICurrentWorkingDirectory
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: shlobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
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
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Shell32.dll
api_name:
 - ICurrentWorkingDirectory
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICurrentWorkingDirectory interface


## -description


Exposes methods that enable a client to retrieve or set an object's current working directory.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ICurrentWorkingDirectory</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>ICurrentWorkingDirectory</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ICurrentWorkingDirectory</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/763c042b-2780-4202-9c3e-073cc8adc93a">GetDirectory</a>
</td>
<td align="left" width="63%">
Gets the current working directory.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/cd7d1517-8c0c-4e42-b750-815fa0aff32c">SetDirectory</a>
</td>
<td align="left" width="63%">
Sets the current working directory.

</td>
</tr>
</table> 


## -remarks



Implement this interface if your object allows clients to retrieve or set the current working directory.

Use this interface to retrieve or set the working directory of the object that exports it.


