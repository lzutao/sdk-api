---
UID: NF:dwrite_3.IDWriteFontSet.FindFontFaceReference
title: IDWriteFontSet::FindFontFaceReference
author: windows-sdk-content
description: Gets the index of the matching font face reference in the font set, with the same file, face index, and simulations.
old-location: directwrite\idwritefontset_findfontfacereference.htm
tech.root: DirectWrite
ms.assetid: dba55a36-8037-5564-59d8-e01189ff0020
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FindFontFaceReference, FindFontFaceReference method [Direct Write], FindFontFaceReference method [Direct Write],IDWriteFontSet interface, IDWriteFontSet interface [Direct Write],FindFontFaceReference method, IDWriteFontSet.FindFontFaceReference, IDWriteFontSet::FindFontFaceReference, directwrite.idwritefontset_findfontfacereference, dwrite_3/IDWriteFontSet::FindFontFaceReference
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dwrite_3.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - IDWriteFontSet.FindFontFaceReference
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontSet::FindFontFaceReference


## -description


Gets the index of the matching font face reference in the font set, with the same file, face index, and simulations.


## -parameters




### -param fontFaceReference

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn894576(v=VS.85).aspx">IDWriteFontFaceReference</a>*</b>

Font face object that specifies the physical font.


### -param listIndex [out]

Type: <b>UINT32*</b>

Receives the zero-based index of the matching font if the font was found, or UINT_MAX otherwise.


### -param exists [out]

Type: <b>BOOL*</b>

Receives TRUE if the font exists or FALSE otherwise.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn933235(v=VS.85).aspx">IDWriteFontSet</a>
 

 
