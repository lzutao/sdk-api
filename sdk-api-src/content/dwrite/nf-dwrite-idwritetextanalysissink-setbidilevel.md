---
UID: NF:dwrite.IDWriteTextAnalysisSink.SetBidiLevel
title: IDWriteTextAnalysisSink::SetBidiLevel
author: windows-sdk-content
description: Sets a bidirectional level on the range, which is called once per run change (either explicit or resolved implicit).
old-location: directwrite\idwritetextanalysissink_setbidilevel.htm
tech.root: DirectWrite
ms.assetid: f51bae22-b4a0-4f72-a341-4479d66cfec5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDWriteTextAnalysisSink interface [Direct Write],SetBidiLevel method, IDWriteTextAnalysisSink.SetBidiLevel, IDWriteTextAnalysisSink::SetBidiLevel, SetBidiLevel, SetBidiLevel method [Direct Write], SetBidiLevel method [Direct Write],IDWriteTextAnalysisSink interface, directwrite.idwritetextanalysissink_setbidilevel, dwrite/IDWriteTextAnalysisSink::SetBidiLevel
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
 - IDWriteTextAnalysisSink.SetBidiLevel
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteTextAnalysisSink::SetBidiLevel


## -description


Sets a bidirectional level on the range, which is  called once per  run change (either explicit or resolved implicit).


## -parameters




### -param textPosition

Type: <b>UINT32</b>

The starting position from which to report.


### -param textLength

Type: <b>UINT32</b>

The number of UTF16 units of the reported range.


### -param explicitLevel

Type: <b>UINT8</b>

The explicit level from the paragraph reading direction and any embedded control codes RLE/RLO/LRE/LRO/PDF, which is determined before any additional rules.


### -param resolvedLevel

Type: <b>UINT8</b>

The final implicit level considering the
         explicit level and characters' natural directionality, after all
         Bidi rules have been applied.


## -returns



Type: <b>HRESULT</b>

A successful code or error code to stop analysis.




## -see-also




<a href="https://msdn.microsoft.com/1fd2ca46-006c-4b01-8258-6c24f4be1641">IDWriteTextAnalysisSink</a>
 

 
