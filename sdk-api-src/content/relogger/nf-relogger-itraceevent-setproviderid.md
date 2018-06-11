---
UID: NF:relogger.ITraceEvent.SetProviderId
title: ITraceEvent::SetProviderId
author: windows-sdk-content
description: Sets the GUID for the provider which traced an event.
old-location: etw\ievent_setproviderid.htm
old-project: ETW
ms.assetid: dc61ff9e-2af9-4428-82df-84635313ddc6
ms.author: windowssdkdev
ms.date: 05/29/2018
ms.keywords: ITraceEvent interface [ETW],SetProviderId method, ITraceEvent.SetProviderId, ITraceEvent::SetProviderId, SetProviderId, SetProviderId method [ETW], SetProviderId method [ETW],ITraceEvent interface, etw.ievent_setproviderid, relogger/ITraceEvent::SetProviderId
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: relogger.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Relogger.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
tech.root: 
req.typenames: RECO_RANGE
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Relogger.h
api_name:
 - ITraceEvent.SetProviderId
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# ITraceEvent::SetProviderId


## -description


The <b>SetProviderId</b> method sets the GUID for the provider which traced an event.


## -parameters




### -param ProviderId [in]

Type: <b>LPCGUID</b>

Unique identifier of the provider.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/29b6f72a-ae81-4292-a023-a4bab16ae143">ITraceEvent</a>
 

 
