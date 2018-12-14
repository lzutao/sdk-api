---
UID: NF:dwrite.IDWriteFontFileEnumerator.MoveNext
title: IDWriteFontFileEnumerator::MoveNext
author: windows-sdk-content
description: Advances to the next font file in the collection. When it is first created, the enumerator is positioned before the first element of the collection and the first call to MoveNext advances to the first file.
old-location: directwrite\IDWriteFontFileEnumerator_MoveNext.htm
tech.root: DirectWrite
ms.assetid: ffacdf0b-2e37-4b69-a6b5-7c6552ecdb60
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDWriteFontFileEnumerator interface [Direct Write],MoveNext method, IDWriteFontFileEnumerator.MoveNext, IDWriteFontFileEnumerator::MoveNext, MoveNext, MoveNext method [Direct Write], MoveNext method [Direct Write],IDWriteFontFileEnumerator interface, directwrite.IDWriteFontFileEnumerator_MoveNext, dwrite/IDWriteFontFileEnumerator::MoveNext
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
 - IDWriteFontFileEnumerator.MoveNext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontFileEnumerator::MoveNext


## -description


 Advances to the next font file in the collection. When it is first created, the enumerator is positioned
     before the first element of the collection and the first call to <b>MoveNext</b> advances to the first file.


## -parameters




### -param hasCurrentFile [out]

Type: <b>BOOL*</b>

When the method returns, contains  the value <b>TRUE</b> if the enumerator advances to a file; otherwise, <b>FALSE</b> if
     the enumerator advances past the last file in the collection.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/d89efffd-ccda-4d55-8419-de142b0f9652">IDWriteFontFileEnumerator</a>
 

 
