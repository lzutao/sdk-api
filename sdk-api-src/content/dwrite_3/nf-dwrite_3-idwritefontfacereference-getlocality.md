---
UID: NF:dwrite_3.IDWriteFontFaceReference.GetLocality
title: IDWriteFontFaceReference::GetLocality
author: windows-sdk-content
description: Get the locality of this font face reference.
old-location: directwrite\idwritefontfacereference_getlocality.htm
tech.root: DirectWrite
ms.assetid: 533f30a7-bf54-670e-63be-ffb9b07fb9d8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetLocality, GetLocality method [Direct Write], GetLocality method [Direct Write],IDWriteFontFaceReference interface, IDWriteFontFaceReference interface [Direct Write],GetLocality method, IDWriteFontFaceReference.GetLocality, IDWriteFontFaceReference::GetLocality, directwrite.idwritefontfacereference_getlocality, dwrite_3/IDWriteFontFaceReference::GetLocality
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dwrite_3.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - IDWriteFontFaceReference.GetLocality
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDWriteFontFaceReference::GetLocality


## -description


Get the locality of this font face reference.


## -parameters






## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Dn890740(v=VS.85).aspx">DWRITE_LOCALITY</a></b>

Returns the locality of this font face reference.




## -remarks



You can always successfully  
     create a font face from a fully local font. Attempting to create a font     
     face on a remote or partially local font may fail with DWRITE_E_REMOTEFONT.    
     This function may change between calls depending on background downloads    
     and whether cached data expires.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn894576(v=VS.85).aspx">IDWriteFontFaceReference</a>
 

 
