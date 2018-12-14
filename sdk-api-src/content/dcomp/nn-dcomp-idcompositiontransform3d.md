---
UID: NN:dcomp.IDCompositionTransform3D
title: IDCompositionTransform3D
author: windows-sdk-content
description: Represents a 3D transformation effect that can be used to modify the rasterization of a visual subtree.
old-location: directcomp\idcompositiontransform3d.htm
tech.root: directcomp
ms.assetid: 81239AB4-C2A3-4E37-95E3-B3C10532EE15
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionTransform3D, IDCompositionTransform3D interface [DirectComposition], IDCompositionTransform3D interface [DirectComposition],described, dcomp/IDCompositionTransform3D, directcomp.idcompositiontransform3d
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
 - IDCompositionTransform3D
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionTransform3D interface


## -description


Represents a 3D transformation effect that can be used to modify the rasterization of a visual subtree. 


## -remarks



The <b>IDCompositionTransform3D</b> interface is an abstract interface that represents a 3D perspective transformation effect. A 3D transform object can be associated with multiple visuals and multiple effect groups. When a 3D transform object is modified, all affected visuals are recomposed to reflect the change.




## -see-also




<a href="https://msdn.microsoft.com/9C9DFECD-0EC0-446C-8CCC-BB7979B01575">IDCompositionEffect</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449159(v=VS.85).aspx">IDCompositionVisual::SetEffect</a>
 

 
