---
UID: NF:dcomp.IDCompositionDevice2.CreateVisual
title: IDCompositionDevice2::CreateVisual
author: windows-sdk-content
description: Creates a new visual object.
old-location: directcomp\idcompositiondevice2_createvisual.htm
tech.root: directcomp
ms.assetid: CCF66B7A-5847-425C-92A4-969C8B915132
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateVisual, CreateVisual method [DirectComposition], CreateVisual method [DirectComposition],IDCompositionDevice2 interface, IDCompositionDevice2 interface [DirectComposition],CreateVisual method, IDCompositionDevice2.CreateVisual, IDCompositionDevice2::CreateVisual, dcomp/IDCompositionDevice2::CreateVisual, directcomp.idcompositiondevice2_createvisual
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: dcomp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps only]
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
 - IDCompositionDevice2.CreateVisual
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionDevice2::CreateVisual


## -description


Creates a new visual object.


## -parameters




### -param visual [out]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh449139(v=VS.85).aspx">IDCompositionVisual</a>**</b>

The new visual object. This parameter must not be NULL.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



A new visual object has a static value of zero for the OffsetX and OffsetY properties, and NULL for the Transform, Clip, and Content properties. Initially, the visual  does not cause the contents of a window to change. The visual must be added as a child of another visual, or as the root of a composition target, before it can affect the appearance of a window.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn280354(v=VS.85).aspx">IDCompositionDevice2</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449109(v=VS.85).aspx">IDCompositionTarget::SetRoot</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449141(v=VS.85).aspx">IDCompositionVisual::AddVisual</a>
 

 
