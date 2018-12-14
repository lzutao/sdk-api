---
UID: NF:hrtfapoapi.IXAPOHrtfParameters.SetSourceGain
title: IXAPOHrtfParameters::SetSourceGain
author: windows-sdk-content
description: Sets the custom direct-path gain value for the current source position. Valid only for sounds played with the HrtfDistanceDecayType custom decay type.
old-location: xaudio2\ixapohrtfparameters_setsourcegain.htm
tech.root: xaudio2
ms.assetid: B1060FF1-6E0F-4B09-BB1B-2517933676D1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IXAPOHrtfParameters interface [XAudio2 Audio Mixing APIs],SetSourceGain method, IXAPOHrtfParameters.SetSourceGain, IXAPOHrtfParameters::SetSourceGain, SetSourceGain, SetSourceGain method [XAudio2 Audio Mixing APIs], SetSourceGain method [XAudio2 Audio Mixing APIs],IXAPOHrtfParameters interface, hrtfapoapi/IXAPOHrtfParameters::SetSourceGain, xaudio2.ixapohrtfparameters_setsourcegain
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: hrtfapoapi.h
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
req.lib: 
req.dll: HrtfApo.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - HrtfApo.dll
api_name:
 - IXAPOHrtfParameters.SetSourceGain
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IXAPOHrtfParameters::SetSourceGain


## -description


Sets the custom direct-path gain value for the current source position. Valid only for sounds played with the HrtfDistanceDecayType custom decay type.


## -parameters




### -param gain [in]

The custom direct-path gain value for the current source position. Valid only for sounds played with the HrtfDistanceDecayType custom decay type.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/EDA29173-84B5-4D2F-90B0-546EEEC49539">IXAPOHrtfParameters</a>
 

 
