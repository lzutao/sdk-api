---
UID: NS:ehstorapi._SILO_INFO
title: SILO_INFO
author: windows-sdk-content
description: SILO_INFO structure contains information that identifies and describes the silo.
old-location: enstor\silo_info.htm
tech.root: enstor
ms.assetid: 8bfe7c31-61e0-420b-8b6b-6b014cd5e243
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PSILO_INFO, PSILO_INFO structure pointer [Enhanced Storage], SILO_INFO, SILO_INFO structure [Enhanced Storage], ehstorapi/PSILO_INFO, ehstorapi/SILO_INFO, enstor.silo_info
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ehstorapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: EhStorAPI.idl
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
 - EhStorAPI.h
api_name:
 - SILO_INFO
product: Windows
targetos: Windows
req.typenames: SILO_INFO
req.redist: 
---

# SILO_INFO structure


## -description


The <b>SILO_INFO</b> structure contains information that identifies and describes the silo.


## -struct-fields




### -field ulSTID

Silo Type Identifier for the silo assigned by IEEE 1667 Working Group.


### -field SpecificationMajor

Major version of the specification implemented in the silo.


### -field SpecificationMinor

Minor version of the specification implemented in the silo.


### -field ImplementationMajor

Major version of the firmware implemented in the silo.


### -field ImplementationMinor

Minor version of the firmware implemented in the silo.


### -field type

Type of the silo.


### -field capabilities

Capabilities of the silo.
