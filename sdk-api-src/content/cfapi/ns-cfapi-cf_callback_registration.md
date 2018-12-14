---
UID: NS:cfapi.CF_CALLBACK_REGISTRATION
title: CF_CALLBACK_REGISTRATION
author: windows-sdk-content
description: The callbacks to be registered by the sync provider.
old-location: cloudapi\cf_callback_registration.htm
tech.root: cfApi
ms.assetid: F1633983-DAB2-4072-AA9E-DC7015E6B988
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CF_CALLBACK_REGISTRATION, CF_CALLBACK_REGISTRATION structure, cfapi/CF_CALLBACK_REGISTRATION, cloudApi.cf_callback_registration
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: cfapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1709 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - CfApi.h
api_name:
 - CF_CALLBACK_REGISTRATION
product: Windows
targetos: Windows
req.typenames: CF_CALLBACK_REGISTRATION
req.redist: 
---

# CF_CALLBACK_REGISTRATION structure


## -description


The callbacks to be registered by the sync provider.


## -struct-fields




### -field Type

The type of callback to be registered.


### -field Callback

A pointer to the callback function.


## -remarks



This callback registration is how a sync provider communicates to the library which functions to call to execute various requests from the platform.

Note that the sync provider only needs to register implemented callbacks, and <b>CF_CALLBACK_REGISTRATION</b> should always end with <b>CF_CALLBACK_REGISTRATION_END</b>.


