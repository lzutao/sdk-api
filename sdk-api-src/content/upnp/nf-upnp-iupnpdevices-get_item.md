---
UID: NF:upnp.IUPnPDevices.get_Item
title: IUPnPDevices::get_Item
author: windows-sdk-content
description: The Item property specifies the IUPnPDevice interface for a device, identified by the UDN, in the collection.
old-location: upnp\iupnpdevices_item.htm
tech.root: upnp
ms.assetid: 38648c9c-6d5a-4215-9270-fd1f893fa360
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IUPnPDevices interface [UPnP APIs],get_Item method, IUPnPDevices.get_Item, IUPnPDevices::get_Item, _upnp_iupnpdevices_item, get_Item, get_Item method [UPnP APIs], get_Item method [UPnP APIs],IUPnPDevices interface, upnp.iupnpdevices_item, upnp/IUPnPDevices::get_Item
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: upnp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
req.dll: Upnp.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Upnp.dll
api_name:
 - IUPnPDevices.get_Item
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IUPnPDevices::get_Item


## -description


The 
<b>Item</b> property specifies the <a href="https://msdn.microsoft.com/566cc606-3dfb-4052-93b0-3c922bf30f84">IUPnPDevice</a> interface for a  device, identified by the UDN, in the collection.


## -parameters




### -param bstrUDN [in]

Specifies a device in the collection.


### -param ppDevice [out]

Receives a reference to an 
<a href="https://msdn.microsoft.com/566cc606-3dfb-4052-93b0-3c922bf30f84">IUPnPDevice</a> interface for the specified device.


## -returns



For C++: If this property's "get" method succeeds, the return value is S_OK. Otherwise, the method returns one of the COM error codes defined in WinError.h.




## -see-also




<a href="https://msdn.microsoft.com/237715dc-2b5a-45b4-b006-d31c0b4e89e3">IUPnPDevices</a>
 

 
