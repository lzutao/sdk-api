---
UID: NE:bthledef._BTH_LE_GATT_DESCRIPTOR_TYPE
title: BTH_LE_GATT_DESCRIPTOR_TYPE
author: windows-sdk-content
description: The BTH_LE_GATT_DESCRIPTOR_TYPE enumeration describes the different types of Bluetooth LE generic attributes (GATT).
old-location: bltooth\bth_le_gatt_descriptor_type.htm
tech.root: bltooth
ms.assetid: 323D649D-B381-4293-BE7C-64651862B9DB
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PBTH_LE_GATT_DESCRIPTOR_TYPE, BTH_LE_GATT_DESCRIPTOR_TYPE, BTH_LE_GATT_DESCRIPTOR_TYPE enumeration [Bluetooth Devices], CharacteristicAggregateFormat, CharacteristicExtendedProperties, CharacteristicFormat, CharacteristicUserDescription, ClientCharacteristicConfiguration, CustomDescriptor, ServerCharacteristicConfiguration, bltooth.bth_le_gatt_descriptor_type, bthledef/BTH_LE_GATT_DESCRIPTOR_TYPE, bthledef/CharacteristicAggregateFormat, bthledef/CharacteristicExtendedProperties, bthledef/CharacteristicFormat, bthledef/CharacteristicUserDescription, bthledef/ClientCharacteristicConfiguration, bthledef/CustomDescriptor, bthledef/ServerCharacteristicConfiguration"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: bthledef.h
req.include-header: BthLEDef.h
req.target-type: Windows
req.target-min-winverclnt: Versions:\_Supported in Windows 8
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - BthLEDef.h
api_name:
 - BTH_LE_GATT_DESCRIPTOR_TYPE
product: Windows
targetos: Windows
req.typenames: BTH_LE_GATT_DESCRIPTOR_TYPE, *PBTH_LE_GATT_DESCRIPTOR_TYPE
req.redist: 
---

# BTH_LE_GATT_DESCRIPTOR_TYPE enumeration


## -description


The BTH_LE_GATT_DESCRIPTOR_TYPE enumeration describes the different types of Bluetooth LE generic attributes (GATT).


## -enum-fields




### -field CharacteristicExtendedProperties

The characteristic value has additional properties that describe how it  can be used, or how it can be accessed.


### -field CharacteristicUserDescription

The characteristic value contains a UTF-8 string of variable size that is a user textual
description.


### -field ClientCharacteristicConfiguration

The characteristic value may be configured by the
client.


### -field ServerCharacteristicConfiguration

The characteristic value may be configured for the
server.


### -field CharacteristicFormat

The format of the characteristic value.


### -field CharacteristicAggregateFormat

The format of an aggregated characteristic value.


### -field CustomDescriptor

The characteristic value is customized.


## -see-also




<a href="https://msdn.microsoft.com/DE738ADA-AE8E-4679-887C-A6194E88386E">BTH_LE_GATT_DESCRIPTOR</a>



<a href="https://msdn.microsoft.com/81D05AA7-B16C-4705-919F-8563FFA4A58E">BTH_LE_GATT_DESCRIPTOR_VALUE</a>
 

 
