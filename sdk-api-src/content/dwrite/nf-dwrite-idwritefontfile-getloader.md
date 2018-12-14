---
UID: NF:dwrite.IDWriteFontFile.GetLoader
title: IDWriteFontFile::GetLoader
author: windows-sdk-content
description: Obtains the file loader associated with a font file object.
old-location: directwrite\IDWriteFontFile_GetLoader.htm
tech.root: DirectWrite
ms.assetid: 60f13a03-2063-4f74-8bfe-217b6c1682ff
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLoader, GetLoader method [Direct Write], GetLoader method [Direct Write],IDWriteFontFile interface, IDWriteFontFile interface [Direct Write],GetLoader method, IDWriteFontFile.GetLoader, IDWriteFontFile::GetLoader, directwrite.IDWriteFontFile_GetLoader, dwrite/IDWriteFontFile::GetLoader
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
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
 - IDWriteFontFile.GetLoader
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontFile::GetLoader


## -description


 Obtains the file loader associated with a font file object.


## -parameters




### -param fontFileLoader [out]

Type: <b><a href="https://msdn.microsoft.com/855e281e-3855-4c11-af87-68f8e0dadbf8">IDWriteFontFileLoader</a>**</b>

When this method returns, contains the address of  a pointer to the font file loader associated with the font file object.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/d4be5466-0b6c-4cc5-9f16-aa00c6037eb9">IDWriteFontFile</a>
 

 
