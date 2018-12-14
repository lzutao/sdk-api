---
UID: NS:wlanapi._WLAN_AVAILABLE_NETWORK_LIST
title: WLAN_AVAILABLE_NETWORK_LIST
author: windows-sdk-content
description: Contains an array of information about available networks.
old-location: nwifi\wlan_available_network_list.htm
tech.root: NativeWiFi
ms.assetid: 0ac508b2-9117-423d-89d3-982f070c70e2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PWLAN_AVAILABLE_NETWORK_LIST, PWLAN_AVAILABLE_NETWORK_LIST, PWLAN_AVAILABLE_NETWORK_LIST structure pointer [NativeWIFI], WLAN_AVAILABLE_NETWORK_LIST, WLAN_AVAILABLE_NETWORK_LIST structure [NativeWIFI], nwifi.wlan_available_network_list, nwifi.wlan_visible_network_list, wlanapi/PWLAN_AVAILABLE_NETWORK_LIST, wlanapi/WLAN_AVAILABLE_NETWORK_LIST"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: wlanapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP3 [desktop apps only]
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
 - wlanapi.h
api_name:
 - WLAN_AVAILABLE_NETWORK_LIST
product: Windows
targetos: Windows
req.typenames: WLAN_AVAILABLE_NETWORK_LIST, *PWLAN_AVAILABLE_NETWORK_LIST
req.redist: Wireless LAN API for Windows XP with SP2
---

# WLAN_AVAILABLE_NETWORK_LIST structure


## -description


The <b>WLAN_AVAILABLE_NETWORK_LIST</b> structure contains an array of information about available networks.


## -struct-fields




### -field dwNumberOfItems

Contains the number of items in the <b>Network</b> member.


### -field dwIndex

The index of the current item.  The index of the first item is 0. <b>dwIndex</b> must be less than <b>dwNumberOfItems</b>.

This member is not used by the wireless service. Applications can use this member when processing individual networks in the   <b>WLAN_AVAILABLE_NETWORK_LIST</b>  structure. When an application passes this structure from one function to another, it can set the value of <b>dwIndex</b> to the index of the item currently being processed. This can help an application maintain state.  

<b>dwIndex</b> should always be initialized before use.


### -field Network.unique

 


### -field Network.size_is

 


### -field Network.size_is.dwNumberOfItems

 


### -field Network

An array of <a href="https://msdn.microsoft.com/82883cea-515b-426d-9961-c144ce99b3db">WLAN_AVAILABLE_NETWORK</a> structures containing interface information.


## -see-also




<a href="https://msdn.microsoft.com/27353a1b-2a3c-4c3b-b512-917d010ee8dd">WlanGetAvailableNetworkList</a>
 

 
