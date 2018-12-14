---
UID: NF:dwrite_1.IDWriteFontFace1.GetMetrics
title: IDWriteFontFace1::GetMetrics
author: windows-sdk-content
description: Obtains design units and common metrics for the font face. These metrics are applicable to all the glyphs within a font face and are used by applications for layout calculations.
old-location: directwrite\idwritefontface1_getmetrics.htm
tech.root: DirectWrite
ms.assetid: 7F899D56-F56B-4C4C-A17D-B42A34CAA0F1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetMetrics, GetMetrics method [Direct Write], GetMetrics method [Direct Write],IDWriteFontFace1 interface, IDWriteFontFace1 interface [Direct Write],GetMetrics method, IDWriteFontFace1.GetMetrics, IDWriteFontFace1::GetMetrics, directwrite.idwritefontface1_getmetrics, dwrite_1/IDWriteFontFace1::GetMetrics
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dwrite_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dwrite_1.lib
req.dll: Dwrite_1.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - dwrite_1.dll
api_name:
 - IDWriteFontFace1.GetMetrics
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontFace1::GetMetrics


## -description


 Obtains design units and common metrics for the font face.
     These metrics are applicable to all the glyphs within a font face and are used by applications for layout calculations.


## -parameters




### -param fontMetrics [out]

Type: <b><a href="https://msdn.microsoft.com/F06033F4-2312-48C2-AF70-BDB83700B4E0">DWRITE_FONT_METRICS1</a>*</b>

A filled <a href="https://msdn.microsoft.com/F06033F4-2312-48C2-AF70-BDB83700B4E0">DWRITE_FONT_METRICS1</a> structure that holds metrics for the current font face element.
     The metrics returned by this method are in font design units.


## -returns



This method does not return a value.




## -see-also




<a href="https://msdn.microsoft.com/1DB7156F-0578-46A0-8C96-E1E34FF4E49E">IDWriteFontFace1</a>
 

 
