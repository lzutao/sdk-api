---
UID: NE:p2p.peer_application_registration_type_tag
title: PEER_APPLICATION_REGISTRATION_TYPE
author: windows-sdk-content
description: The PEER_APPLICATION_REGISTRATION_TYPE enumeration defines the set of peer application registration flags.
old-location: p2p\peer_application_registration_type.htm
tech.root: P2PSdk
ms.assetid: 58f14e46-377e-494b-93ef-fc19e8d87fcc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PEER_APPLICATION_ALL_USERS, PEER_APPLICATION_CURRENT_USER, PEER_APPLICATION_REGISTRATION_TYPE, PEER_APPLICATION_REGISTRATION_TYPE enumeration [Peer Networking], p2p.peer_application_registration_type, p2p/PEER_APPLICATION_ALL_USERS, p2p/PEER_APPLICATION_CURRENT_USER, p2p/PEER_APPLICATION_REGISTRATION_TYPE
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: p2p.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: None supported
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
 - PEER_APPLICATION_REGISTRATION_TYPE
product: Windows
targetos: Windows
req.typenames: PEER_APPLICATION_REGISTRATION_TYPE
req.redist: 
---

# PEER_APPLICATION_REGISTRATION_TYPE enumeration


## -description


The <b>PEER_APPLICATION_REGISTRATION_TYPE</b> enumeration defines the set of peer application registration flags.


## -enum-fields




### -field PEER_APPLICATION_CURRENT_USER

The application is available only to the current user account logged into the machine.


### -field PEER_APPLICATION_ALL_USERS

The application is available to all user accounts set on the machine.


## -remarks



"Peer application" defines the set of software applications or components available for use with the peer collaboration network. The peer collaboration network enables participants in the network to initiate usage of this application.

Applications with the same GUID and registered for the <b>current user</b>  take precedence over applications with that same GUID registered for <b>all users</b>.




## -see-also




<a href="https://msdn.microsoft.com/f72e372a-0d23-47f4-8518-1296ec81ce55">Collaboration API Enumerations</a>
 

 
