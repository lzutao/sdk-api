---
UID: NS:ipsectypes.IPSEC_TUNNEL_ENDPOINT0_
title: IPSEC_TUNNEL_ENDPOINT0
author: windows-sdk-content
description: Used to store address information for an end point of a tunnel mode SA.
old-location: fwp\ipsec_tunnel_endpoint0.htm
tech.root: fwp
ms.assetid: e536e9b0-1128-4548-9461-3cdeba509873
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IPSEC_TUNNEL_ENDPOINT0, IPSEC_TUNNEL_ENDPOINT0 structure [Filtering], fwp.ipsec_tunnel_endpoint0, ipsectypes/IPSEC_TUNNEL_ENDPOINT0
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ipsectypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Ipsectypes.idl
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
 - ipsectypes.h
api_name:
 - IPSEC_TUNNEL_ENDPOINT0
product: Windows
targetos: Windows
req.typenames: IPSEC_TUNNEL_ENDPOINT0
req.redist: 
---

# IPSEC_TUNNEL_ENDPOINT0 structure


## -description


The <b>IPSEC_TUNNEL_ENDPOINT0</b> structure is used to store address information for an end point of a tunnel mode SA.


## -struct-fields




### -field ipVersion

Type: <b><a href="https://msdn.microsoft.com/1712b83c-f32d-4981-9950-ab870a376182">FWP_IP_VERSION</a></b>

Specifies the IP version. In tunnel mode, this is the version of the outer header.


### -field v4Address

 


### -field v6Address

 




#### - ( unnamed union )

switch_type(FWP_IP_VERSION), switch_is(ipVersion)

Tagged union containing the tunnel end point address.



#### v4Address

<b>Type: <b>UINT32</b>
</b>
case(FWP_IP_VERSION_V4)



#### v6Address

<b>Type: <b>UINT8[16]</b>
</b>
case(FWP_IP_VERSION_V6)


## -remarks



<b>IPSEC_TUNNEL_ENDPOINT0</b> is a specific implementation of IPSEC_TUNNEL_ENDPOINT. See <a href="https://msdn.microsoft.com/FBDF53E5-F7DE-4DEB-AC18-6D2BB59FE670">WFP Version-Independent Names and Targeting Specific Versions of Windows</a>  for more information.




## -see-also




<a href="https://msdn.microsoft.com/1712b83c-f32d-4981-9950-ab870a376182">FWP_IP_VERSION</a>



<a href="https://msdn.microsoft.com/091daec1-2c35-4d24-89be-fcdb0354b674">IPSEC_TUNNEL_ENDPOINTS2</a>



<a href="https://msdn.microsoft.com/e957132f-417b-40c1-afe3-5aec0e2192f7">Windows Filtering Platform  API Structures</a>
 

 
