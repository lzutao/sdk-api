---
UID: NE:icftypes.NET_FW_SERVICE_TYPE_
title: NET_FW_SERVICE_TYPE
author: windows-sdk-content
description: Specifies the type of service.
old-location: ics\net_fw_service_type.htm
tech.root: ics
ms.assetid: c2d7c143-8b89-41a8-8c5f-ac1e90ca5215
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: NET_FW_SERVICE_FILE_AND_PRINT, NET_FW_SERVICE_NONE, NET_FW_SERVICE_REMOTE_DESKTOP, NET_FW_SERVICE_TYPE, NET_FW_SERVICE_TYPE enumeration [ICS/ICF], NET_FW_SERVICE_TYPE_MAX, NET_FW_SERVICE_UPNP, icftypes/NET_FW_SERVICE_FILE_AND_PRINT, icftypes/NET_FW_SERVICE_NONE, icftypes/NET_FW_SERVICE_REMOTE_DESKTOP, icftypes/NET_FW_SERVICE_TYPE, icftypes/NET_FW_SERVICE_TYPE_MAX, icftypes/NET_FW_SERVICE_UPNP, ics.net_fw_service_type
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: icftypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only]
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
 - Icftypes.h
api_name:
 - NET_FW_SERVICE_TYPE
product: Windows
targetos: Windows
req.typenames: NET_FW_SERVICE_TYPE
req.redist: 
---

# NET_FW_SERVICE_TYPE enumeration


## -description


<p class="CCE_Message">[The Windows Firewall API is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions. For Windows Vista and later, use of the <a href="https://msdn.microsoft.com/8F33B96B-AA9A-46d5-8808-0F2D0723935B">Windows Firewall with Advanced Security</a> API is recommended.]

The 
<b>NET_FW_SERVICE_TYPE</b> enumerated type specifies the type of service.


## -enum-fields




### -field NET_FW_SERVICE_FILE_AND_PRINT

Service type is File and Print Sharing.


### -field NET_FW_SERVICE_UPNP

Service type is UPnP Framework.


### -field NET_FW_SERVICE_REMOTE_DESKTOP

Service type is Remote Desktop.


### -field NET_FW_SERVICE_NONE

Not a valid service type. This is used to indicate that a port is not part of a service.


### -field NET_FW_SERVICE_TYPE_MAX

Used for boundary checking only. Not valid for application programming.


## -see-also




<a href="https://msdn.microsoft.com/9a0c1e65-68d6-4e64-bc95-2b83d8db3c43">Windows Firewall Enumerated Types</a>



<a href="https://msdn.microsoft.com/bcc8b1ef-a11e-4e8e-9519-fe8cb73e1abe">Windows Firewall Reference</a>
 

 
