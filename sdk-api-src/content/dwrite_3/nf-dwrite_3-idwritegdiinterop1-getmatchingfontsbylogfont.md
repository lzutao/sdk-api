---
UID: NF:dwrite_3.IDWriteGdiInterop1.GetMatchingFontsByLOGFONT
title: IDWriteGdiInterop1::GetMatchingFontsByLOGFONT
author: windows-sdk-content
description: Gets a list of matching fonts based on the specified LOGFONT values. Only fonts of that family name will be returned.
old-location: directwrite\idwritegdiinterop1_getmatchingfontsbylogfont.htm
tech.root: DirectWrite
ms.assetid: 38D547D2-0C1C-4673-83BD-38458DFD7E5A
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetMatchingFontsByLOGFONT, GetMatchingFontsByLOGFONT method [Direct Write], GetMatchingFontsByLOGFONT method [Direct Write],IDWriteGdiInterop1 interface, IDWriteGdiInterop1 interface [Direct Write],GetMatchingFontsByLOGFONT method, IDWriteGdiInterop1.GetMatchingFontsByLOGFONT, IDWriteGdiInterop1::GetMatchingFontsByLOGFONT, directwrite.idwritegdiinterop1_getmatchingfontsbylogfont, dwrite_3/IDWriteGdiInterop1::GetMatchingFontsByLOGFONT
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
 - IDWriteGdiInterop1.GetMatchingFontsByLOGFONT
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteGdiInterop1::GetMatchingFontsByLOGFONT


## -description


Gets a list of matching fonts based on the specified LOGFONT values. Only fonts
        of that family name will be returned.


## -parameters




### -param logFont [in]

Type: <b>LOGFONT</b>

Structure containing a GDI-compatible font description.


### -param fontSet [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn933235(v=VS.85).aspx">IDWriteFontSet</a>*</b>

The font set to search.


### -param filteredSet [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn933235(v=VS.85).aspx">IDWriteFontSet</a>**</b>

&gt;Receives the filtered font set if successful.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn958415(v=VS.85).aspx">IDWriteGdiInterop1</a>
 

 
