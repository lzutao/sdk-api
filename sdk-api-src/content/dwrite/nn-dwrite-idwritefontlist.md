---
UID: NN:dwrite.IDWriteFontList
title: IDWriteFontList
author: windows-sdk-content
description: Represents a list of fonts.
old-location: directwrite\IDWriteFontList.htm
tech.root: DirectWrite
ms.assetid: 00c41c5f-4405-45ff-98e5-03858dc3056f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDWriteFontList, IDWriteFontList interface [Direct Write], IDWriteFontList interface [Direct Write],described, directwrite.IDWriteFontList, dwrite/IDWriteFontList
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: dwrite.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
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
 - IDWriteFontList
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontList interface


## -description


 Represents a list of fonts.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDWriteFontList</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IDWriteFontList</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDWriteFontList</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b2262707-b5d5-4697-9634-72fd2a72000a">GetFont</a>
</td>
<td align="left" width="63%">
 Gets a font given its zero-based index.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/f3c13a33-7bf7-4027-af10-f4863008cef2">GetFontCollection</a>
</td>
<td align="left" width="63%">
 Gets the font collection that contains the fonts in
    the font list.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/62755704-f4bf-423c-b19b-781529dd9718">GetFontCount</a>
</td>
<td align="left" width="63%">
 Gets the number of fonts in the font list.

</td>
</tr>
</table> 
