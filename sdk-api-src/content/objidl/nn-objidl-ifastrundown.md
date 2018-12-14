---
UID: NN:objidl.IFastRundown
title: IFastRundown
author: windows-sdk-content
description: Marks an interface as eligible for fast rundown behavior.
old-location: com\ifastrundown.htm
tech.root: com
ms.assetid: 8406B781-7CBE-47F8-B7EF-5FF599BB8EDE
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFastRundown, IFastRundown interface [COM], IFastRundown interface [COM],described, com.ifastrundown, objidl/IFastRundown
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: objidl.h
req.include-header: Objidlbase.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Objidlbase.idl
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
 - COM
api_location:
 - objidl.h
api_name:
 - IFastRundown
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFastRundown interface


## -description


Marks an interface as eligible for fast rundown behavior.


## -remarks



A Component Object Model (COM) object implements the <b>IFastRundown</b> marker interface to opt into the fast rundown behavior.

All Windows Store app processes, as well as the broker processes RuntimeBroker.exe and PickerHost.exe, apply fast rundown at the process level, which means that all objects in any of these processes are subjected to fast rundown automatically. Desktop processes don't get this behavior by default and must opt in at the process level. Specific objects opt in by implementing the <b>IFastRundown</b> marker interface.




## -see-also




<a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a>
 

 
