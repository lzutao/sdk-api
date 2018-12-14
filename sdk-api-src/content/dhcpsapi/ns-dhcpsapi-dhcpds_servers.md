---
UID: NS:dhcpsapi._DHCPDS_SERVERS
title: DHCPDS_SERVERS
author: windows-sdk-content
description: The DHCPDS_SERVERS structure defines a list of DHCP servers in the context of directory services.
old-location: dhcp\dhcpds_servers.htm
tech.root: DHCP
ms.assetid: 0f5fe4f3-4eaa-498b-ab48-bfb5ee8f5527
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPDHCPDS_SERVERS, *PDHCPDS_SERVERS, DHCPDS_SERVERS, DHCPDS_SERVERS structure [DHCP], DHCP_SERVER_INFO_ARRAY, DHCP_SERVER_INFO_ARRAY structure [DHCP], LPDHCPDS_SERVERS *PDHCPDS_SERVERS, LPDHCPDS_SERVERS *PDHCPDS_SERVERS structure pointer [DHCP], LPDHCP_SERVER_INFO_ARRAY *PDHCP_SERVER_INFO_ARRAY, LPDHCP_SERVER_INFO_ARRAY *PDHCP_SERVER_INFO_ARRAY structure pointer [DHCP], PDHCPDS_SERVERS, PDHCPDS_SERVERS structure pointer [DHCP], PDHCP_SERVER_INFO_ARRAY, PDHCP_SERVER_INFO_ARRAY structure pointer [DHCP], dhcp.dhcpds_servers, dhcpsapi/DHCP_SERVER_INFO_ARRAY, dhcpsapi/LPDHCPDS_SERVERS *PDHCPDS_SERVERS, dhcpsapi/LPDHCP_SERVER_INFO_ARRAY *PDHCP_SERVER_INFO_ARRAY, dhcpsapi/PDHCPDS_SERVERS, dhcpsapi/PDHCP_SERVER_INFO_ARRAY, dhcpsapi/_DHCPDS_SERVERS"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: dhcpsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - DHCPDS_SERVERS
product: Windows
targetos: Windows
req.typenames: DHCPDS_SERVERS, *LPDHCPDS_SERVERS, *PDHCPDS_SERVERS
req.redist: 
---

# DHCPDS_SERVERS structure


## -description


The <b>DHCPDS_SERVERS</b> structure defines a list of DHCP servers in the context of directory services.


## -struct-fields




### -field Flags

Reserved. This value should be 0.


### -field NumElements

Specifies the number of elements in <b>Servers</b>.


### -field Servers

Pointer to an array of <a href="https://msdn.microsoft.com/12f3fbd3-9b81-4a11-914c-83658c2bce89">DHCPDS_SERVER</a> structures that contain information on individual DHCP servers.
