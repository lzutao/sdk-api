---
UID: NF:dwrite.IDWriteLocalFontFileLoader.GetFilePathFromKey
title: IDWriteLocalFontFileLoader::GetFilePathFromKey
author: windows-sdk-content
description: Obtains the absolute font file path from the font file reference key.
old-location: directwrite\idwritelocalfontfileloader_getfilepathfromkey.htm
tech.root: DirectWrite
ms.assetid: a61cfe80-100d-4813-b04f-a39f626893dd
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetFilePathFromKey, GetFilePathFromKey method [Direct Write], GetFilePathFromKey method [Direct Write],IDWriteLocalFontFileLoader interface, IDWriteLocalFontFileLoader interface [Direct Write],GetFilePathFromKey method, IDWriteLocalFontFileLoader.GetFilePathFromKey, IDWriteLocalFontFileLoader::GetFilePathFromKey, directwrite.idwritelocalfontfileloader_getfilepathfromkey, dwrite/IDWriteLocalFontFileLoader::GetFilePathFromKey
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
 - IDWriteLocalFontFileLoader.GetFilePathFromKey
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteLocalFontFileLoader::GetFilePathFromKey


## -description


Obtains the absolute font file path from the font file reference key.


## -parameters




### -param fontFileReferenceKey [in]

Type: <b>const void*</b>

The font file reference key that uniquely identifies the local font file
    within the scope of the font loader being used.


### -param fontFileReferenceKeySize

Type: <b>UINT32</b>

The size of font file reference key in bytes.


### -param filePath [out]

Type: <b>WCHAR*</b>

The character array that receives the local file path.


### -param filePathSize

Type: <b>UINT32</b>

The length of the file path character array.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/acb777c8-24c6-452e-8f58-8fb2ad8c0b6c">IDWriteLocalFontFileLoader</a>
 

 
