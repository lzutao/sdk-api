---
UID: NF:dwrite.IDWriteTextLayout.DetermineMinWidth
title: IDWriteTextLayout::DetermineMinWidth
author: windows-sdk-content
description: Determines the minimum possible width the layout can be set to without emergency breaking between the characters of whole words occurring.
old-location: directwrite\idwritetextlayout_determineminwidth.htm
tech.root: DirectWrite
ms.assetid: 8efa1471-1b74-46d4-ac6d-fb1839ce2e74
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DetermineMinWidth, DetermineMinWidth method [Direct Write], DetermineMinWidth method [Direct Write],IDWriteTextLayout interface, IDWriteTextLayout interface [Direct Write],DetermineMinWidth method, IDWriteTextLayout.DetermineMinWidth, IDWriteTextLayout::DetermineMinWidth, directwrite.idwritetextlayout_determineminwidth, dwrite/IDWriteTextLayout::DetermineMinWidth
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dwrite.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dwrite.lib
req.dll: Dwrite.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - dwrite.dll
api_name:
 - IDWriteTextLayout.DetermineMinWidth
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteTextLayout::DetermineMinWidth


## -description


Determines the minimum possible width the layout can be set to without emergency breaking between the characters of whole words occurring.


## -parameters




### -param minWidth [out]

Type: <b>FLOAT*</b>

Minimum width.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/0d687337-8623-4014-967c-f533072e31cc">IDWriteTextLayout</a>
 

 
