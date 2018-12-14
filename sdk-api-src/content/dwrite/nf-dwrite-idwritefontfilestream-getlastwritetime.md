---
UID: NF:dwrite.IDWriteFontFileStream.GetLastWriteTime
title: IDWriteFontFileStream::GetLastWriteTime
author: windows-sdk-content
description: Obtains the last modified time of the file.
old-location: directwrite\IDWriteFontFileStream_GetLastWriteTime.htm
tech.root: DirectWrite
ms.assetid: eb4045c0-a333-40aa-8ec3-b89cfd835be3
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLastWriteTime, GetLastWriteTime method [Direct Write], GetLastWriteTime method [Direct Write],IDWriteFontFileStream interface, IDWriteFontFileStream interface [Direct Write],GetLastWriteTime method, IDWriteFontFileStream.GetLastWriteTime, IDWriteFontFileStream::GetLastWriteTime, directwrite.IDWriteFontFileStream_GetLastWriteTime, dwrite/IDWriteFontFileStream::GetLastWriteTime
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
 - IDWriteFontFileStream.GetLastWriteTime
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontFileStream::GetLastWriteTime


## -description


 Obtains the last modified time of the file. 


## -parameters




### -param lastWriteTime [out]

Type: <b>UINT64*</b>

When this method returns, contains  the last modified time of the file in the format that represents
     the number of 100-nanosecond intervals since January 1, 1601 (UTC).


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The "last modified time" is used by DirectWrite font selection algorithms
     to determine whether one font resource is more up to date than another one.




## -see-also




<a href="https://msdn.microsoft.com/792ab9be-853f-427d-a762-2da8e81423f8">IDWriteFontFileStream</a>
 

 
