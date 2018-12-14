---
UID: NF:dwrite.IDWriteFontFace.GetGdiCompatibleGlyphMetrics
title: IDWriteFontFace::GetGdiCompatibleGlyphMetrics
author: windows-sdk-content
description: Obtains glyph metrics in font design units with the return values compatible with what GDI would produce.
old-location: directwrite\idwritefontface_getgdicompatibleglyphmetrics.htm
tech.root: DirectWrite
ms.assetid: 7bda3916-6db3-4f56-b18c-288506c0b646
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetGdiCompatibleGlyphMetrics, GetGdiCompatibleGlyphMetrics method [Direct Write], GetGdiCompatibleGlyphMetrics method [Direct Write],IDWriteFontFace interface, IDWriteFontFace interface [Direct Write],GetGdiCompatibleGlyphMetrics method, IDWriteFontFace.GetGdiCompatibleGlyphMetrics, IDWriteFontFace::GetGdiCompatibleGlyphMetrics, directwrite.idwritefontface_getgdicompatibleglyphmetrics, dwrite/IDWriteFontFace::GetGdiCompatibleGlyphMetrics
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
 - IDWriteFontFace.GetGdiCompatibleGlyphMetrics
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontFace::GetGdiCompatibleGlyphMetrics


## -description


Obtains glyph metrics in font design units with the return values compatible with what GDI would produce.


## -parameters




### -param emSize

Type: <b>FLOAT</b>

The ogical size of the font in DIP units.


### -param pixelsPerDip

Type: <b>FLOAT</b>

The number of physical pixels per DIP.


### -param transform [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/fe4bd8ba-fc3b-4a04-8a72-9983d52f4404">DWRITE_MATRIX</a>*</b>

An optional transform applied to the glyphs and their positions. This transform is applied after the
    scaling specified by the font size and <i>pixelsPerDip</i>.


### -param useGdiNatural

Type: <b>BOOL</b>

When set to <b>FALSE</b>, the metrics are the same as the metrics of GDI aliased text.  When set to <b>TRUE</b>, the metrics are the same as the metrics of text measured by GDI using a font created with <b>CLEARTYPE_NATURAL_QUALITY</b>.


### -param glyphIndices [in]

Type: <b>const UINT16*</b>

An array of glyph indices for which to compute the metrics.


### -param glyphCount

Type: <b>UINT32</b>

The number of elements in the <i>glyphIndices</i> array.


### -param glyphMetrics [out]

Type: <b><a href="https://msdn.microsoft.com/d2a4ac9f-f510-4235-93bb-e7bdecc65873">DWRITE_GLYPH_METRICS</a>*</b>

An array of <a href="https://msdn.microsoft.com/d2a4ac9f-f510-4235-93bb-e7bdecc65873">DWRITE_GLYPH_METRICS</a> structures filled by this function. The metrics are in font design units.


### -param isSideways

Type: <b>BOOL</b>

A BOOL value that indicates whether the font is being used in a sideways run.  This can affect the glyph metrics if the font has oblique simulation because sideways oblique simulation differs from non-sideways oblique simulation.


## -returns



Type: <b>HRESULT</b>

Standard <b>HRESULT</b> error code. If any of the input glyph indices are outside of the valid glyph index range for the current font face, <b>E_INVALIDARG</b> will be returned.




## -see-also




<a href="https://msdn.microsoft.com/1b6bb9e2-cf01-413c-9ee8-42bb0f703ce8">IDWriteFontFace</a>
 

 
