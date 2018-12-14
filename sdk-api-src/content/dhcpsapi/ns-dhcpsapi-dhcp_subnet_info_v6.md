---
UID: NS:dhcpsapi._DHCP_SUBNET_INFO_V6
title: DHCP_SUBNET_INFO_V6
author: windows-sdk-content
description: Contains information about an IPv6 subnet.
old-location: dhcp\dhcp_subnet_info_v6.htm
tech.root: DHCP
ms.assetid: cd60f9d0-3ac3-4661-aefe-ddb9052db3e1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPDHCP_SUBNET_INFO_V6, *PDHCP_SUBNET_INFO_V6, DHCP_SUBNET_INFO_V6, DHCP_SUBNET_INFO_V6 structure [DHCP], PDHCP_SUBNET_INFO_V6, PDHCP_SUBNET_INFO_V6 structure pointer [DHCP], dhcp.dhcp_subnet_info_v6, dhcpsapi/DHCP_SUBNET_INFO_V6, dhcpsapi/PDHCP_SUBNET_INFO_V6"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: dhcpsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008, Windows Server 2008 R2 [desktop apps only]
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
 - Dhcpsapi.h
api_name:
 - DHCP_SUBNET_INFO_V6
product: Windows
targetos: Windows
req.typenames: DHCP_SUBNET_INFO_V6, *PDHCP_SUBNET_INFO_V6, *LPDHCP_SUBNET_INFO_V6
req.redist: 
---

# DHCP_SUBNET_INFO_V6 structure


## -description


The <b>DHCP_SUBNET_INFO_V6</b> structure contains information about an IPv6 subnet.


## -struct-fields




### -field SubnetAddress


<a href="https://msdn.microsoft.com/9623e866-81e5-4d5a-8801-33f0f8973ed3">DHCP_IPV6_ADDRESS</a> structure containing the IPv6 prefix.


### -field Prefix

<b>ULONG</b> value that specifies the length of the IPv6 prefix.


### -field Preference

<b>USHORT</b> value that specifies the preference for the IPv6 prefix.


### -field SubnetName

Pointer to a null-terminated Unicode string that contains the name of the IPv6 prefix.


### -field SubnetComment

Pointer to a null-terminated Unicode string that contains an optional comment for the IPv6 prefix.


### -field State

An enumeration of the <a href="https://msdn.microsoft.com/1f2960ae-98f2-4c93-9705-e8b74a4f5e21">DHCP_SUBNET_STATE</a> that indicates the current state of the IPv6 prefix.


### -field ScopeId

A <b>DWORD</b> value that serves as the unique identifier for the IPv6 prefix. This value is generated by the DHCPv6 server.


## -see-also




<a href="https://msdn.microsoft.com/9623e866-81e5-4d5a-8801-33f0f8973ed3">DHCP_IPV6_ADDRESS</a>
 

 
