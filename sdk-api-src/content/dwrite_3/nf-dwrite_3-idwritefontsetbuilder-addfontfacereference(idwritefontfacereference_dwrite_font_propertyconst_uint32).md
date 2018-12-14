---
UID: NF:dwrite_3.IDWriteFontSetBuilder.AddFontFaceReference(IDWriteFontFaceReference,DWRITE_FONT_PROPERTY const,UINT32)
title: IDWriteFontSetBuilder::AddFontFaceReference(IDWriteFontFaceReference,DWRITE_FONT_PROPERTY const,UINT32)
author: windows-sdk-content
description: Adds a reference to a font to the set being built. The necessary metadata will automatically be extracted from the font upon calling CreateFontSet.
old-location: directwrite\idwritefontsetbuilder_addfontfacereference_1.htm
tech.root: DirectWrite
ms.assetid: 0E67F5EF-F8BB-47D9-995D-40879351DC17
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AddFontFaceReference, AddFontFaceReference method [Direct Write], AddFontFaceReference method [Direct Write],IDWriteFontSetBuilder interface, IDWriteFontSetBuilder interface [Direct Write],AddFontFaceReference method, IDWriteFontSetBuilder.AddFontFaceReference, IDWriteFontSetBuilder.AddFontFaceReference(IDWriteFontFaceReference,DWRITE_FONT_PROPERTY const,UINT32), IDWriteFontSetBuilder::AddFontFaceReference, IDWriteFontSetBuilder::AddFontFaceReference(IDWriteFontFaceReference,DWRITE_FONT_PROPERTY const,UINT32), directwrite.idwritefontsetbuilder_addfontfacereference_1, dwrite_3/IDWriteFontSetBuilder::AddFontFaceReference
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dwrite_3.h
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
 - IDWriteFontSetBuilder.AddFontFaceReference
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontSetBuilder::AddFontFaceReference(IDWriteFontFaceReference,DWRITE_FONT_PROPERTY const,UINT32)


## -description


Adds a reference to a font to the set being built. The necessary metadata will automatically be extracted from the font upon calling CreateFontSet.


## -parameters




### -param fontFaceReference [in]

Type: <b><a href="https://msdn.microsoft.com/04242508-7439-43B6-B3E7-07617B782038">IDWriteFontFaceReference</a>*</b>

Font face reference object to add to the set.


### -param properties

TBD


### -param propertyCount

TBD




## -returns



Type: <b><a href="455d07e9-52c3-4efb-a9dc-2955cbfd38cc">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/CC6C95CA-BA8B-47C4-A241-650EC8477192">IDWriteFontSetBuilder</a>
 

 
