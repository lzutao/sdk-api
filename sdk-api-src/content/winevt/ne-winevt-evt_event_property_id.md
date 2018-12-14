---
UID: NE:winevt._EVT_EVENT_PROPERTY_ID
title: EVT_EVENT_PROPERTY_ID
author: windows-sdk-content
description: Defines the values that determine the query information to retrieve.
old-location: wes\evt_subscription_event_property_id.htm
tech.root: wes
ms.assetid: 19e20da3-5b6b-4f56-b30b-0408695f2267
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EVT_EVENT_PROPERTY_ID, EVT_EVENT_PROPERTY_ID enumeration [EventLog], EvtEventPath, EvtEventPropertyIdEND, EvtEventQueryIDs, wes.evt_subscription_event_property_id, winevt/EVT_EVENT_PROPERTY_ID, winevt/EvtEventPath, winevt/EvtEventPropertyIdEND, winevt/EvtEventQueryIDs
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: winevt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - WinEvt.h
api_name:
 - EVT_EVENT_PROPERTY_ID
product: Windows
targetos: Windows
req.typenames: EVT_EVENT_PROPERTY_ID
req.redist: 
---

# EVT_EVENT_PROPERTY_ID enumeration


## -description


Defines the values that determine the query information to retrieve.


## -enum-fields




### -field EvtEventQueryIDs

Not supported. The identifier of the query that selected the event. The variant type of this property is EvtVarTypeInt32.


### -field EvtEventPath

The channel or log file from which the event came. The variant type of this property is EvtVarTypeString.


### -field EvtEventPropertyIdEND

This enumeration value marks the end of the enumeration values. It can be used to exit a loop when retrieving all the properties.


## -see-also




<a href="https://msdn.microsoft.com/69aa22a1-10c1-43bd-ae3b-d7641bed2065">EvtGetEventInfo</a>
 

 
