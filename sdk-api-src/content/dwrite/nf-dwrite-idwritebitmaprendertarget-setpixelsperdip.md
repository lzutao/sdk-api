---
UID: NF:dwrite.IDWriteBitmapRenderTarget.SetPixelsPerDip
title: IDWriteBitmapRenderTarget::SetPixelsPerDip
author: windows-sdk-content
description: Sets the number of bitmap pixels per DIP (device-independent pixel). A DIP is 1/96 inch, so this value is the number if pixels per inch divided by 96.
old-location: directwrite\IDWriteBitmapRenderTarget_SetPixelsPerDip.htm
tech.root: DirectWrite
ms.assetid: da582190-4a6d-451a-9d42-831e8786570f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDWriteBitmapRenderTarget interface [Direct Write],SetPixelsPerDip method, IDWriteBitmapRenderTarget.SetPixelsPerDip, IDWriteBitmapRenderTarget::SetPixelsPerDip, SetPixelsPerDip, SetPixelsPerDip method [Direct Write], SetPixelsPerDip method [Direct Write],IDWriteBitmapRenderTarget interface, directwrite.IDWriteBitmapRenderTarget_SetPixelsPerDip, dwrite/IDWriteBitmapRenderTarget::SetPixelsPerDip
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
 - IDWriteBitmapRenderTarget.SetPixelsPerDip
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteBitmapRenderTarget::SetPixelsPerDip


## -description


 Sets the number of bitmap pixels per DIP (device-independent pixel). A DIP is 1/96 inch, so this value is the number
     if pixels per inch divided by 96.


## -parameters




### -param pixelsPerDip

Type: <b>FLOAT</b>

A value that specifies the number of pixels per DIP.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/9953a9e9-7772-41a3-9cd9-2340a9dd4b6f">IDWriteBitmapRenderTarget</a>
 

 
