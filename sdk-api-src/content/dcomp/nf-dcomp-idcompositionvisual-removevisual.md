---
UID: NF:dcomp.IDCompositionVisual.RemoveVisual
title: IDCompositionVisual::RemoveVisual
author: windows-sdk-content
description: Removes a child visual from the children list of this visual.
old-location: directcomp\idcompositionvisual_removevisual.htm
tech.root: directcomp
ms.assetid: d77161b1-cb35-40a7-a51c-4b44ea320e78
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionVisual interface [DirectComposition],RemoveVisual method, IDCompositionVisual.RemoveVisual, IDCompositionVisual::RemoveVisual, RemoveVisual, RemoveVisual method [DirectComposition], RemoveVisual method [DirectComposition],IDCompositionVisual interface, dcomp/IDCompositionVisual::RemoveVisual, directcomp.idcompositionvisual_removevisual
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
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
 - IDCompositionVisual.RemoveVisual
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionVisual::RemoveVisual


## -description


Removes a child visual from the children list of this visual.


## -parameters




### -param visual [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh449139(v=VS.85).aspx">IDCompositionVisual</a>*</b>

The child visual to remove from the children list. This parameter must not be NULL.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If the function succeeds, it returns S_OK. Otherwise, it returns an <b>HRESULT</b> error code. See <a href="https://msdn.microsoft.com/8DFBFC34-DBD0-4731-8305-B33E90C96C54">DirectComposition Error Codes</a>  for a list of error codes.




## -remarks



The child visual is removed from the list of children. The order of the remaining child visuals is not changed.

This method fails if <i>visual</i> is not a child of the parent visual.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Hh437414(v=VS.85).aspx">IDCompositionDevice::CreateVisual</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449139(v=VS.85).aspx">IDCompositionVisual</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449141(v=VS.85).aspx">IDCompositionVisual::AddVisual</a>



<a href="https://msdn.microsoft.com/en-us/library/Hh449143(v=VS.85).aspx">IDCompositionVisual::RemoveAllVisuals</a>
 

 
