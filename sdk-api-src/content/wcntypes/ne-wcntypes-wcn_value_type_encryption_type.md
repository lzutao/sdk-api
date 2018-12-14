---
UID: NE:wcntypes.tagWCN_VALUE_TYPE_ENCRYPTION_TYPE
title: WCN_VALUE_TYPE_ENCRYPTION_TYPE
author: windows-sdk-content
description: WCN_VALUE_TYPE_ENCRYPTION_TYPE enumeration defines the supported WLAN encryption types.
old-location: wcn\wcn_value_type_encryption_type.htm
tech.root: wcn
ms.assetid: 4bd6ef62-82cd-4d3d-925a-637396452c03
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WCN_VALUE_ET_AES, WCN_VALUE_ET_NONE, WCN_VALUE_ET_TKIP, WCN_VALUE_ET_TKIP_AES_MIXED, WCN_VALUE_ET_WEP, WCN_VALUE_TYPE_ENCRYPTION_TYPE, WCN_VALUE_TYPE_ENCRYPTION_TYPE enumeration [Windows Connect Now], wcn.wcn_value_type_encryption_type, wcntypes/WCN_VALUE_ET_AES, wcntypes/WCN_VALUE_ET_NONE, wcntypes/WCN_VALUE_ET_TKIP, wcntypes/WCN_VALUE_ET_TKIP_AES_MIXED, wcntypes/WCN_VALUE_ET_WEP, wcntypes/WCN_VALUE_TYPE_ENCRYPTION_TYPE
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: wcntypes.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
 - wcntypes.h
api_name:
 - WCN_VALUE_TYPE_ENCRYPTION_TYPE
product: Windows
targetos: Windows
req.typenames: WCN_VALUE_TYPE_ENCRYPTION_TYPE
req.redist: 
---

# WCN_VALUE_TYPE_ENCRYPTION_TYPE enumeration


## -description


The <b>WCN_VALUE_TYPE_ENCRYPTION_TYPE</b> enumeration defines the supported WLAN encryption types.


## -enum-fields




### -field WCN_VALUE_ET_NONE

Specifies support for unsecured wireless activity.


### -field WCN_VALUE_ET_WEP

Specifies support for the Wired Equivalent Privacy (WEP) encryption method.

<div class="alert"><b>Note</b>  Not available for WPS 2.0.</div>
<div> </div>

### -field WCN_VALUE_ET_TKIP

Specifies support for the Temporal Key Integrity Protocol (TKIP) encryption method.

<div class="alert"><b>Note</b>  Not available for WPS 2.0.</div>
<div> </div>

### -field WCN_VALUE_ET_AES

Specifies support for the Advanced Encryption Standard (AES) encryption method.


### -field WCN_VALUE_ET_TKIP_AES_MIXED

Specifies support for WPAPSK/WPA2PSK mixed-mode encryption.

<div class="alert"><b>Note</b>  Not supported in WPS 1.0. Only available  in Windows 8.</div>
<div> </div>

## -see-also




<a href="https://msdn.microsoft.com/214b64c3-b1f0-46b1-b52a-b1df1bb40cf7">WCN_ATTRIBUTE_TYPE</a>
 

 
