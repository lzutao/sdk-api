---
UID: NN:dcomp.IDCompositionEffect
title: IDCompositionEffect
author: windows-sdk-content
description: Represents a bitmap effect that modifies the rasterization of a visual's subtree.
old-location: directcomp\idcompositioneffect.htm
tech.root: directcomp
ms.assetid: 9C9DFECD-0EC0-446C-8CCC-BB7979B01575
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionEffect, IDCompositionEffect interface [DirectComposition], IDCompositionEffect interface [DirectComposition],described, dcomp/IDCompositionEffect, directcomp.idcompositioneffect
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: dcomp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - IDCompositionEffect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionEffect interface


## -description


Represents a bitmap effect that modifies the rasterization of a visual's subtree.




## -remarks



<b>IDCompositionEffect</b> is an abstract interface that represents a bitmap effect. An effect applies to the entire visual subtree rooted at the visual that the effect is associated with. An effect object can be associated with multiple visuals. When an effect object is modified, all affected visuals are recomposed to reflect the change.



More than one effect can be simultaneously applied to a visual by using the <a href="https://msdn.microsoft.com/en-us/library/Hh437418(v=VS.85).aspx">IDCompositionEffectGroup</a> interface.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh449159(v=VS.85).aspx">IDCompositionVisual::SetEffect</a>
 

 
