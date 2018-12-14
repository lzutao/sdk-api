---
UID: NF:dwrite_3.IDWriteStringList.GetString
title: IDWriteStringList::GetString
author: windows-sdk-content
description: Copies the string with the specified index to the specified array.
old-location: directwrite\idwritestringlist_getstring.htm
tech.root: DirectWrite
ms.assetid: 9F569418-F5CF-4280-8E53-32F14AE6FD42
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetString, GetString method [Direct Write], GetString method [Direct Write],IDWriteStringList interface, IDWriteStringList interface [Direct Write],GetString method, IDWriteStringList.GetString, IDWriteStringList::GetString, directwrite.idwritestringlist_getstring, dwrite_3/IDWriteStringList::GetString
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
 - IDWriteStringList.GetString
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteStringList::GetString


## -description


Copies the string with the specified index to the specified array.


## -parameters




### -param listIndex

Type: <b>UINT32</b>

Zero-based index of the string.


### -param stringBuffer [out]

Type: <b>WCHAR*</b>

Character array that receives the string.


### -param stringBufferSize

Type: <b>UINT32</b>

Size of the array in characters. The size must include space for the terminating null character.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn958421(v=VS.85).aspx">IDWriteStringList</a>
 

 
