---
UID: NF:relogger.ITraceEvent.SetEventDescriptor
title: ITraceEvent::SetEventDescriptor
author: windows-sdk-content
description: Sets the event descriptor for an event.
old-location: etw\ievent_seteventdescriptor.htm
old-project: ETW
ms.assetid: 729a887e-1759-44d5-a7d5-8385d648eebf
ms.author: windowssdkdev
ms.date: 05/29/2018
ms.keywords: ITraceEvent interface [ETW],SetEventDescriptor method, ITraceEvent.SetEventDescriptor, ITraceEvent::SetEventDescriptor, SetEventDescriptor, SetEventDescriptor method [ETW], SetEventDescriptor method [ETW],ITraceEvent interface, etw.ievent_seteventdescriptor, relogger/ITraceEvent::SetEventDescriptor
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
 - ITraceEvent.SetEventDescriptor
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# ITraceEvent::SetEventDescriptor


## -description


The <b>SetEventDescriptor</b> method sets the event descriptor for an event.


## -parameters




### -param EventDescriptor [in]

Type: <b><a href="https://msdn.microsoft.com/907e6c38-5eaa-49da-9dc0-d055dcc69d1a">PCEVENT_DESCRIPTOR</a></b>

The event descriptor data.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/907e6c38-5eaa-49da-9dc0-d055dcc69d1a">EVENT_DESCRIPTOR</a>



<a href="https://msdn.microsoft.com/29b6f72a-ae81-4292-a023-a4bab16ae143">ITraceEvent</a>
 

 
