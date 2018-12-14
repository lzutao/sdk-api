---
UID: NF:dwrite.IDWriteTextFormat.GetLineSpacing
title: IDWriteTextFormat::GetLineSpacing
author: windows-sdk-content
description: Gets the line spacing adjustment set for a multiline text paragraph.
old-location: directwrite\IDWriteTextFormat_GetLineSpacing.htm
tech.root: DirectWrite
ms.assetid: d9563d4d-0b7d-4921-b251-6ef1e24105f1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLineSpacing, GetLineSpacing method [Direct Write], GetLineSpacing method [Direct Write],IDWriteTextFormat interface, IDWriteTextFormat interface [Direct Write],GetLineSpacing method, IDWriteTextFormat.GetLineSpacing, IDWriteTextFormat::GetLineSpacing, directwrite.IDWriteTextFormat_GetLineSpacing, dwrite/IDWriteTextFormat::GetLineSpacing
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
 - IDWriteTextFormat.GetLineSpacing
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteTextFormat::GetLineSpacing


## -description


 Gets the line spacing adjustment set for a multiline text paragraph.


## -parameters




### -param lineSpacingMethod [out]

Type: <b><a href="https://msdn.microsoft.com/b75e8fee-ed6c-455d-8733-e6972792572c">DWRITE_LINE_SPACING_METHOD</a>*</b>

A value that indicates how line height is determined.


### -param lineSpacing [out]

Type: <b>FLOAT*</b>

When this method returns, contains the line height, or  distance between one baseline to another.


### -param baseline [out]

Type: <b>FLOAT*</b>

When this method returns, contains the distance from top of line to baseline. A reasonable ratio to <i>lineSpacing</i> is 80 percent.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/64b2cac3-c4cb-4213-b808-7b279d296939">IDWriteTextFormat</a>
 

 
