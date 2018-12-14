---
UID: NF:dwrite.IDWriteTextAnalyzer.GetGdiCompatibleGlyphPlacements
title: IDWriteTextAnalyzer::GetGdiCompatibleGlyphPlacements
author: windows-sdk-content
description: Place glyphs output from the GetGlyphs method according to the font and the writing system's rendering rules.
old-location: directwrite\idwritetextanalyzer_getgdicompatibleglyphplacements.htm
tech.root: DirectWrite
ms.assetid: 49312b03-9ee9-44ef-b3eb-a35631a6e693
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetGdiCompatibleGlyphPlacements, GetGdiCompatibleGlyphPlacements method [Direct Write], GetGdiCompatibleGlyphPlacements method [Direct Write],IDWriteTextAnalyzer interface, IDWriteTextAnalyzer interface [Direct Write],GetGdiCompatibleGlyphPlacements method, IDWriteTextAnalyzer.GetGdiCompatibleGlyphPlacements, IDWriteTextAnalyzer::GetGdiCompatibleGlyphPlacements, directwrite.idwritetextanalyzer_getgdicompatibleglyphplacements, dwrite/IDWriteTextAnalyzer::GetGdiCompatibleGlyphPlacements
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
 - IDWriteTextAnalyzer.GetGdiCompatibleGlyphPlacements
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteTextAnalyzer::GetGdiCompatibleGlyphPlacements


## -description


Place glyphs output from the <a href="https://msdn.microsoft.com/9bc373b6-9161-4ffc-a942-50d97d6509c3">GetGlyphs</a> method according to the font 
    and the writing system's rendering rules.


## -parameters




### -param textString [in]

Type: <b>const WCHAR*</b>

An array of characters containing the original string from which the glyphs came.


### -param clusterMap [in]

Type: <b>const UINT16*</b>

A pointer to the mapping from character ranges to glyph 
     ranges. This is returned by <a href="https://msdn.microsoft.com/9bc373b6-9161-4ffc-a942-50d97d6509c3">GetGlyphs</a>.


### -param textProps [in]

Type: <b><a href="https://msdn.microsoft.com/2fd1af73-c2ea-4077-9cf5-77ab9f237f0a">DWRITE_SHAPING_TEXT_PROPERTIES</a>*</b>

A pointer to an array of structures that contains  shaping properties for each character. This structure is returned by 
     <a href="https://msdn.microsoft.com/9bc373b6-9161-4ffc-a942-50d97d6509c3">GetGlyphs</a>.


### -param textLength

Type: <b>UINT32</b>

The text length of <i>textString</i>.


### -param glyphIndices [in]

Type: <b>const UINT16*</b>

An array of glyph indices returned by <a href="https://msdn.microsoft.com/9bc373b6-9161-4ffc-a942-50d97d6509c3">GetGlyphs</a>.


### -param glyphProps [in]

Type: <b>const <a href="https://msdn.microsoft.com/debaa84f-8883-4117-9be0-962857b55020">DWRITE_SHAPING_GLYPH_PROPERTIES</a>*</b>

A pointer to an array of structures that contain  shaping properties for each glyph returned by <a href="https://msdn.microsoft.com/9bc373b6-9161-4ffc-a942-50d97d6509c3">GetGlyphs</a>.


### -param glyphCount

Type: <b>UINT32</b>

The number of glyphs returned from <a href="https://msdn.microsoft.com/9bc373b6-9161-4ffc-a942-50d97d6509c3">GetGlyphs</a>.


### -param fontFace [in]

Type: <b><a href="https://msdn.microsoft.com/1b6bb9e2-cf01-413c-9ee8-42bb0f703ce8">IDWriteFontFace</a>*</b>

A pointer to the font face that is the source for the output glyphs.


### -param fontEmSize

Type: <b>FLOAT</b>

The logical font size in DIPs.


### -param pixelsPerDip

Type: <b>FLOAT</b>

The number of physical pixels per DIP.


### -param transform [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/fe4bd8ba-fc3b-4a04-8a72-9983d52f4404">DWRITE_MATRIX</a>*</b>

An optional transform applied to the glyphs and their positions. This transform is applied after the scaling specified by the font size and <i>pixelsPerDip</i>.


### -param useGdiNatural

Type: <b>BOOL</b>

When set to <b>FALSE</b>, the metrics are the same as the metrics of GDI aliased text.  When set to <b>TRUE</b>, the metrics are the same as the metrics of text measured by GDI using a font created with <b>CLEARTYPE_NATURAL_QUALITY</b>.


### -param isSideways

Type: <b>BOOL</b>

A Boolean flag set to <b>TRUE</b> if the text is intended to be
     drawn vertically.


### -param isRightToLeft

Type: <b>BOOL</b>

A Boolean flag set to <b>TRUE</b> for right-to-left text.


### -param scriptAnalysis [in]

Type: <b>const <a href="https://msdn.microsoft.com/dafda5f6-39aa-4577-9213-898bdeddc7c2">DWRITE_SCRIPT_ANALYSIS</a>*</b>

A pointer to a Script analysis result from an<a href="https://msdn.microsoft.com/e681f7c8-7d87-454b-a7b6-6c3fe38b0f92">AnalyzeScript</a> call.


### -param localeName [in, optional]

Type: <b>const WCHAR*</b>

An array of characters containing the locale to use when selecting glyphs.
     For example, the same character may map to different glyphs for ja-jp versus zh-chs.
     If this is <b>NULL</b>, then the default mapping based on the script is used.


### -param features [in, optional]

Type: <b>const <a href="https://msdn.microsoft.com/21ef4266-5dd6-48b6-9175-452b74e94a07">DWRITE_TYPOGRAPHIC_FEATURES</a>**</b>

An array of pointers to the sets of typographic 
     features to use in each feature range.


### -param featureRangeLengths [in, optional]

Type: <b>const UINT32*</b>

The length of each feature range, in characters.  
     The sum of all lengths should be equal to <i>textLength</i>.


### -param featureRanges

Type: <b>UINT32</b>

The number of feature ranges.


### -param glyphAdvances [out]

Type: <b>FLOAT*</b>

When this method returns, contains the advance width of each glyph.


### -param glyphOffsets [out]

Type: <b><a href="https://msdn.microsoft.com/f5a231c0-78df-4fe0-99a8-81fcad517cda">DWRITE_GLYPH_OFFSET</a>*</b>

When this method returns, contains the offset of the origin of each glyph.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/e832ffc4-31db-41b1-a008-04696d9a975e">IDWriteTextAnalyzer</a>
 

 
