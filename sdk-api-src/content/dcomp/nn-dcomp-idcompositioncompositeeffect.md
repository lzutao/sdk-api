---
UID: NN:dcomp.IDCompositionCompositeEffect
title: IDCompositionCompositeEffect
author: windows-sdk-content
description: The composite effect is used to combine 2 or more images.
old-location: directcomp\idcompositioncompositeeffect.htm
tech.root: directcomp
ms.assetid: 72647FCE-F1B0-4A50-927B-23EE38EEEC8B
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionCompositeEffect, IDCompositionCompositeEffect interface [DirectComposition], IDCompositionCompositeEffect interface [DirectComposition],described, dcomp/IDCompositionCompositeEffect, directcomp.idcompositioncompositeeffect
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
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
 - IDCompositionCompositeEffect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionCompositeEffect interface


## -description


The composite effect is used to combine 2 or more images. This effect has 13 different composite modes.
          The composite effect accepts 2 or more inputs. When you specify 2 images, destination is the first input (index 0) and the source is the second input (index 1). 
          If you specify more than 2 inputs, the images are composited starting with the first input and the second and so on.
        


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDCompositionCompositeEffect</b> interface inherits from <a href="https://msdn.microsoft.com/en-us/library/Dn919730(v=VS.85).aspx">IDCompositionFilterEffect</a>. <b>IDCompositionCompositeEffect</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDCompositionCompositeEffect</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dn919729(v=VS.85).aspx">SetMode</a>
</td>
<td align="left" width="63%">
Sets the mode for the composite effect.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn919730(v=VS.85).aspx">IDCompositionFilterEffect</a>
 

 
