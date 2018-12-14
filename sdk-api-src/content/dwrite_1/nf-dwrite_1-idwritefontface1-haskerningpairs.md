---
UID: NF:dwrite_1.IDWriteFontFace1.HasKerningPairs
title: IDWriteFontFace1::HasKerningPairs
author: windows-sdk-content
description: Determines whether the font supports pair-kerning.
old-location: directwrite\idwritefontface1_haskerningpairs.htm
tech.root: DirectWrite
ms.assetid: 701B874A-BA95-43CA-8762-70BA571FDC10
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: HasKerningPairs, HasKerningPairs method [Direct Write], HasKerningPairs method [Direct Write],IDWriteFontFace1 interface, IDWriteFontFace1 interface [Direct Write],HasKerningPairs method, IDWriteFontFace1.HasKerningPairs, IDWriteFontFace1::HasKerningPairs, directwrite.idwritefontface1_haskerningpairs, dwrite_1/IDWriteFontFace1::HasKerningPairs
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
 - IDWriteFontFace1.HasKerningPairs
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontFace1::HasKerningPairs


## -description


Determines whether the font supports pair-kerning.


## -parameters






## -returns



Returns TRUE if the font supports kerning pairs, otherwise FALSE.




## -remarks



If the font doesn't support pair table kerning, you don't need to
    call <a href="https://msdn.microsoft.com/DA837B04-85BC-4A3B-A6FE-24D5AFD21B14">IDWriteFontFace1::GetKerningPairAdjustments</a> because it would retrieve all zeroes.




## -see-also




<a href="https://msdn.microsoft.com/1DB7156F-0578-46A0-8C96-E1E34FF4E49E">IDWriteFontFace1</a>



<a href="https://msdn.microsoft.com/DA837B04-85BC-4A3B-A6FE-24D5AFD21B14">IDWriteFontFace1::GetKerningPairAdjustments</a>
 

 
