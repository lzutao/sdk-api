---
UID: NF:dcomp.IDCompositionTurbulenceEffect.SetNoise
title: IDCompositionTurbulenceEffect::SetNoise
author: windows-sdk-content
description: Sets the turbulence noise mode.
old-location: directcomp\idcompositionturbulenceeffect_setnoise.htm
tech.root: directcomp
ms.assetid: 6EF5C8D0-C614-4520-BAE5-A3C8E609FB64
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionTurbulenceEffect interface [DirectComposition],SetNoise method, IDCompositionTurbulenceEffect.SetNoise, IDCompositionTurbulenceEffect::SetNoise, SetNoise, SetNoise method [DirectComposition], SetNoise method [DirectComposition],IDCompositionTurbulenceEffect interface, dcomp/IDCompositionTurbulenceEffect::SetNoise, directcomp.idcompositionturbulenceeffect_setnoise
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dcomp.h
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
req.lib: Dcomp.lib
req.dll: Dcomp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Dcomp.dll
api_name:
 - IDCompositionTurbulenceEffect.SetNoise
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionTurbulenceEffect::SetNoise


## -description


Sets the turbulence noise mode.


## -parameters




### -param noise [in]

Type: <b><a href="https://msdn.microsoft.com/86C1990E-958C-46D7-840A-E4A17F1D1740">D2D1_TURBULENCE_NOISE</a></b>

The turbulence noise mode. Indicates whether to generate a bitmap based on Fractal Noise or the Turbulence function.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn919801(v=VS.85).aspx">IDCompositionTurbulenceEffect</a>
 

 
