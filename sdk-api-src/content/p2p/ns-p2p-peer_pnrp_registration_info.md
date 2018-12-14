---
UID: NS:p2p.peer_pnrp_registration_info_tag
title: PEER_PNRP_REGISTRATION_INFO
author: windows-sdk-content
description: Contains the information provided by a peer identity when it registers with a PNRP cloud.
old-location: p2p\peer_pnrp_registration_info.htm
tech.root: P2PSdk
ms.assetid: 2825cb65-94b4-4bed-acff-7fa35a992284
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PPEER_PNRP_REGISTRATION_INFO, PEER_PNRP_REGISTRATION_INFO, PEER_PNRP_REGISTRATION_INFO structure [Peer Networking], PPEER_PNRP_REGISTRATION_INFO, PPEER_PNRP_REGISTRATION_INFO structure pointer [Peer Networking], p2p.peer_pnrp_registration_info, p2p/PEER_PNRP_REGISTRATION_INFO, p2p/PPEER_PNRP_REGISTRATION_INFO"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: p2p.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only],Windows XP with SP1 with the Advanced Networking Pack for Windows XP
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
 - P2P.h
api_name:
 - PEER_PNRP_REGISTRATION_INFO
product: Windows
targetos: Windows
req.typenames: PEER_PNRP_REGISTRATION_INFO, *PPEER_PNRP_REGISTRATION_INFO
req.redist: 
---

# PEER_PNRP_REGISTRATION_INFO structure


## -description


The <b>PEER_PNRP_REGISTRATION_INFO</b> structure contains the information provided by a peer identity when it registers with a PNRP cloud.


## -struct-fields




### -field pwzCloudName

Pointer to a Unicode string that contains the name of the PNRP cloud for which this peer identity is requesting registration. If <b>NULL</b>, the registration will be made in all clouds.  It is possible to use the special value PEER_PNRP_ALL_LINK_CLOUDS to register in all link local clouds.


### -field pwzPublishingIdentity

Pointer to a Unicode string that contains the name of the peer identity requesting registration.


### -field cAddresses

The number of SOCKADDR structures in <b>ppAddresses</b>. It is possible to use the special value PEER_PNRP_AUTO_ADDRESSES to have the infrastructure automatically choose addresses.


### -field ppAddresses

Pointer to an array of pointers to SOCKADDR structures that contain the IP addresses bound to the network interface of the peer identity requesting registration.


### -field wPort

The network interface port assigned to the address that the peer is publishing.


### -field pwzComment

Pointer to a zero-terminated Unicode string that contains a comment for this peer endpoint.


### -field payload

A <a href="https://msdn.microsoft.com/d8a8b9e3-c455-4813-b812-263efe7f5e3e">PEER_DATA</a> structure that contains a pointer to an opaque byte buffer containing application-specific data for the peer endpoint (such as a message or an image).
