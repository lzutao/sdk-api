---
UID: NS:winioctl._STORAGE_PHYSICAL_ADAPTER_DATA
title: STORAGE_PHYSICAL_ADAPTER_DATA
author: windows-sdk-content
description: Describes a physical storage adapter.
old-location: fs\storage_physical_adapter_data.htm
tech.root: fileio
ms.assetid: 8CC7CF43-61C8-4561-BA9C-473878818858
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSTORAGE_PHYSICAL_ADAPTER_DATA, PSTORAGE_PHYSICAL_ADAPTER_DATA, PSTORAGE_PHYSICAL_ADAPTER_DATA structure pointer [Files], STORAGE_PHYSICAL_ADAPTER_DATA, STORAGE_PHYSICAL_ADAPTER_DATA structure [Files], fs.storage_physical_adapter_data, winioctl/PSTORAGE_PHYSICAL_ADAPTER_DATA, winioctl/STORAGE_PHYSICAL_ADAPTER_DATA"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winioctl.h
req.include-header: Windows.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - WinIoCtl.h
api_name:
 - STORAGE_PHYSICAL_ADAPTER_DATA
product: Windows
targetos: Windows
req.typenames: STORAGE_PHYSICAL_ADAPTER_DATA, *PSTORAGE_PHYSICAL_ADAPTER_DATA
req.redist: 
---

# STORAGE_PHYSICAL_ADAPTER_DATA structure


## -description


Describes a physical storage adapter.


## -struct-fields




### -field AdapterId

Specifies the adapter ID.


### -field HealthStatus

A <a href="https://msdn.microsoft.com/ECC5A745-EA8B-4FBE-840D-0D959C9ED5BA">STORAGE_COMPONENT_HEALTH_STATUS</a>-typed value. 


### -field CommandProtocol

A <a href="https://msdn.microsoft.com/8055B633-99EF-4AAE-AA80-FC09F357BEAB">STORAGE_PROTOCOL_TYPE</a>-typed value.


### -field SpecVersion

A <a href="https://msdn.microsoft.com/470DBBC0-A7D7-42A6-97D0-44AEAC990576">STORAGE_SPEC_VERSION</a>-typed value that specifies the supported storage spec version (for example, AHCI 1.3.1).


### -field Vendor

 


### -field Model

 


### -field FirmwareRevision

 


### -field PhysicalLocation

 


### -field ExpanderConnected

Indicates whether an expander is connected.


### -field Reserved0

 


### -field Reserved1

 




#### - FirmwareRevision[16]

Specifies the firmware revision.


#### - Model[40]

Specifies the adapter model.


#### - PhysicalLocation[32]

Reserved for future use.


#### - Reserved0[3]

Reserved.


#### - Reserved1[3]

Reserved.


#### - Vendor[8]

Specifies the adapter vendor.
