---
UID: NS:dhcpsapi._DHCP_FAILOVER_STATISTICS
title: DHCP_FAILOVER_STATISTICS
author: windows-sdk-content
description: The DHCP_FAILOVER_STATISTICS structure defines DHCP server scope statistics that are part of a failover relationship.
old-location: dhcp\dhcp_failover_statistics.htm
tech.root: DHCP
ms.assetid: a06d873c-fc82-40c1-be3e-45f24328897d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPDHCP_FAILOVER_STATISTICS, DHCP_FAILOVER_STATISTICS, DHCP_FAILOVER_STATISTICS structure [DHCP], LPDHCP_FAILOVER_STATISTICS, LPDHCP_FAILOVER_STATISTICS structure pointer [DHCP], dhcp.dhcp_failover_statistics, dhcpsapi/DHCP_FAILOVER_STATISTICS, dhcpsapi/LPDHCP_FAILOVER_STATISTICS"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: dhcpsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - dhcpsapi.h
api_name:
 - DHCP_FAILOVER_STATISTICS
product: Windows
targetos: Windows
req.typenames: DHCP_FAILOVER_STATISTICS, *LPDHCP_FAILOVER_STATISTICS
req.redist: 
---

# DHCP_FAILOVER_STATISTICS structure


## -description


The <b>DHCP_FAILOVER_STATISTICS</b> structure defines DHCP server scope statistics that are part of a failover relationship.


## -struct-fields




### -field NumAddr

 


### -field AddrFree

 


### -field AddrInUse

 


### -field PartnerAddrFree

 


### -field ThisAddrFree

 


### -field PartnerAddrInUse

 


### -field ThisAddrInUse

 




#### - addrFree

Value that specifies the total number of free IPv4 addresses that can be leased out to clients in a DHCPv4 scope that are part of a failover relationship.


#### - addrInUse

Value that specifies the total number of IPv4 addresses that are leased out to clients in a DHCPv4 scope that are part of a failover relationship.


#### - numAddr

Value that specifies the total number of addresses in a DHCPv4 scope that are part of a failover relationship.


#### - partnerAddrFree

Value that specifies the number of free IPv4 addresses on the partner server that can be leased out to clients in a DHCPv4 scope that are part of a failover relationship.


#### - partnerAddrInUse

Value that specifies the number of IPv4 addresses on the partner server that are leased out to clients in a DHCPv4 scope that are part of a failover relationship.


#### - thisAddrFree

Value that specifies the number of free IPv4 addresses on the local server that can be leased out to clients in a DHCPv4 scope that are part of a failover relationship.


#### - thisAddrInUse

Value that specifies the number of IPv4 addresses on the local server that are leased out to clients in a DHCPv4 scope that are part of a failover relationship.


## -see-also




<a href="https://msdn.microsoft.com/888945a8-5c07-440a-ad2d-2126342facda">DhcpV4FailoverGetScopeStatistics</a>
 

 
