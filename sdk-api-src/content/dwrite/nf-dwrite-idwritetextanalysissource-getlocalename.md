---
UID: NF:dwrite.IDWriteTextAnalysisSource.GetLocaleName
title: IDWriteTextAnalysisSource::GetLocaleName
author: windows-sdk-content
description: Gets the locale name on the range affected by the text analysis.
old-location: directwrite\idwritetextanalysissource_getlocalename.htm
tech.root: DirectWrite
ms.assetid: 88a2474b-c14d-41ce-9687-f498644c0315
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLocaleName, GetLocaleName method [Direct Write], GetLocaleName method [Direct Write],IDWriteTextAnalysisSource interface, IDWriteTextAnalysisSource interface [Direct Write],GetLocaleName method, IDWriteTextAnalysisSource.GetLocaleName, IDWriteTextAnalysisSource::GetLocaleName, directwrite.idwritetextanalysissource_getlocalename, dwrite/IDWriteTextAnalysisSource::GetLocaleName
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
 - IDWriteTextAnalysisSource.GetLocaleName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteTextAnalysisSource::GetLocaleName


## -description


Gets the locale name on the range affected by the text analysis.


## -parameters




### -param textPosition

Type: <b>UINT32</b>

The text position to examine.


### -param textLength [out]

Type: <b>UINT32*</b>

Contains the length of the text being affected by the text analysis up to the next differing locale.


### -param localeName [out]

Type: <b>const WCHAR**</b>

Contains an address of a  pointer to an array of characters which receives the locale name from the text affected by the text analysis. The array of characters is null-terminated.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The <i>localeName</i> pointer must remain valid until the next call or until the analysis returns.




## -see-also




<a href="https://msdn.microsoft.com/7e2a523d-9191-4f99-9e73-a7955c432126">IDWriteTextAnalysisSource</a>
 

 
