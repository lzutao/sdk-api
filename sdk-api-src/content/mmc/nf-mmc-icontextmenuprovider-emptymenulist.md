---
UID: NF:mmc.IContextMenuProvider.EmptyMenuList
title: IContextMenuProvider::EmptyMenuList
author: windows-sdk-content
description: The IContextMenuProvider::EmptyMenuList method clears a context menu.
old-location: mmc\icontextmenuprovider_emptymenulist.htm
tech.root: mmc
ms.assetid: d8867d95-4812-499b-81cd-d0f9471fe33b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EmptyMenuList, EmptyMenuList method [MMC], EmptyMenuList method [MMC],IContextMenuProvider interface, IContextMenuProvider interface [MMC],EmptyMenuList method, IContextMenuProvider.EmptyMenuList, IContextMenuProvider::EmptyMenuList, _slate_icontextmenuprovider_emptymenulist, mmc.icontextmenuprovider_emptymenulist, mmc/IContextMenuProvider::EmptyMenuList
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mmc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: Mmcndmgr.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mmcndmgr.dll
api_name:
 - IContextMenuProvider.EmptyMenuList
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IContextMenuProvider::EmptyMenuList


## -description


The <b>IContextMenuProvider::EmptyMenuList</b> method clears a context menu.


## -parameters






## -returns



This method can return one of these values.




## -remarks




<a href="https://msdn.microsoft.com/8fe9f474-c47b-4b53-8cbc-d658c82d7591">IContextMenuProvider::ShowContextMenu</a> automatically clears the context menu after that displays it. Nevertheless, it is a good practice to call 
<b>EmptyMenuList</b> before beginning to build a context menu.




## -see-also




<a href="https://msdn.microsoft.com/3f9a5945-9b34-41fe-9c91-c782eb7eb739">IContextMenuProvider</a>
 

 
