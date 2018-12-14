---
UID: NS:dhcpcsdk._DHCPAPI_PARAMS
title: DHCPAPI_PARAMS
author: windows-sdk-content
description: The DHCPAPI_PARAMS structure is used to request DHCP parameters.
old-location: dhcp\dhcpapi_params.htm
tech.root: DHCP
ms.assetid: be8329a3-c3ad-4f5b-92ae-cf18fa847d53
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPDHCPAPI_PARAMS, *LPDHCPAPI_PARAMS structure [DHCP], *LPDHCPCAPI_PARAMS, *LPDHCPCAPI_PARAMS structure [DHCP], *PDHCPAPI_PARAMS, *PDHCPAPI_PARAMS structure [DHCP], *PDHCPCAPI_PARAMS, *PDHCPCAPI_PARAMS structure [DHCP], DHCPAPI_PARAMS, DHCPAPI_PARAMS structure [DHCP], DHCPCAPI_PARAMS, DHCPCAPI_PARAMS structure [DHCP], dhcp.dhcpapi_params, dhcpcsdk/*LPDHCPAPI_PARAMS, dhcpcsdk/*LPDHCPCAPI_PARAMS, dhcpcsdk/*PDHCPAPI_PARAMS, dhcpcsdk/*PDHCPCAPI_PARAMS, dhcpcsdk/DHCPAPI_PARAMS, dhcpcsdk/DHCPCAPI_PARAMS"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: dhcpcsdk.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
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
 - Dhcpcsdk.h
api_name:
 - DHCPAPI_PARAMS
product: Windows
targetos: Windows
req.typenames: DHCPAPI_PARAMS, *PDHCPAPI_PARAMS, *LPDHCPAPI_PARAMS, DHCPCAPI_PARAMS, *PDHCPCAPI_PARAMS, *LPDHCPCAPI_PARAMS
req.redist: 
---

# DHCPAPI_PARAMS structure


## -description


The <b>DHCPAPI_PARAMS</b> structure is used to request DHCP parameters.


## -struct-fields




### -field Flags

Reserved. Must be set to zero.


### -field OptionId

Identifier for the DHCP parameter being requested.


### -field IsVendor

Specifies whether the DHCP parameter is vendor-specific. Set to <b>TRUE</b> if the parameter is vendor-specific.


### -field Data.size_is

 


### -field Data.size_is.nBytesData

 


### -field Data

Pointer to the parameter data.


### -field nBytesData

Size of the data pointed to by <b>Data</b>, in bytes.


## -see-also




<a href="https://msdn.microsoft.com/84eafc6b-e9ee-4c73-b872-b2abc7e257df">DHCPAPI_PARAMS_ARRAY</a>
 

 
