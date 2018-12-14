---
UID: NF:dcomp.IDCompositionHueRotationEffect.SetAngle(IDCompositionAnimation)
title: IDCompositionHueRotationEffect::SetAngle(IDCompositionAnimation)
author: windows-sdk-content
description: Sets the angle to rotate the hue.
old-location: directcomp\idcompositionhuerotationeffect_setangle_2.htm
tech.root: directcomp
ms.assetid: F0D73D46-D649-47F3-B1F1-FD995228A3EC
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IDCompositionHueRotationEffect interface [DirectComposition],SetAngle method, IDCompositionHueRotationEffect.SetAngle, IDCompositionHueRotationEffect.SetAngle(IDCompositionAnimation), IDCompositionHueRotationEffect::SetAngle, IDCompositionHueRotationEffect::SetAngle(IDCompositionAnimation), SetAngle, SetAngle method [DirectComposition], SetAngle method [DirectComposition],IDCompositionHueRotationEffect interface, dcomp/IDCompositionHueRotationEffect::SetAngle, directcomp.idcompositionhuerotationeffect_setangle_2
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
 - IDCompositionHueRotationEffect.SetAngle
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IDCompositionHueRotationEffect::SetAngle(IDCompositionAnimation)


## -description


Sets the angle to rotate the hue.


## -parameters




### -param animation [in]

Type: <b><a href="https://msdn.microsoft.com/f914e14b-4ac0-4591-9b7f-6b45b88baaaa">IDCompositionAnimation</a>*</b>

An animation that represents how the angle value changes over time. 
          The effect calculates a color matrix based on the rotation angle (θ) according to the following matrix equations:
          

<img alt="Matrix equation" src="./images/hue_formula.png"/>
This parameter must not be NULL.


## -returns



Type: <b><a href="https://msdn.microsoft.com/en-us/library/Hh437604(v=VS.85).aspx">HRESULT</a></b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dn919738(v=VS.85).aspx">IDCompositionHueRotationEffect</a>
 

 
