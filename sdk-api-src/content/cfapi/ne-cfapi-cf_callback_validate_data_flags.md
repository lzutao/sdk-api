---
UID: NE:cfapi.CF_CALLBACK_VALIDATE_DATA_FLAGS
title: CF_CALLBACK_VALIDATE_DATA_FLAGS
author: windows-sdk-content
description: Flags to validate the data of a placeholder file or directory.
old-location: cloudapi\cf_callback_validate_data_flags.htm
tech.root: cfApi
ms.assetid: D5BEAEAA-318E-4BA5-8DC5-EDD24E2C26EF
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CF_CALLBACK_VALIDATE_DATA_FLAGS, CF_CALLBACK_VALIDATE_DATA_FLAGS enumeration, CF_CALLBACK_VALIDATE_DATA_FLAG_EXPLICIT_HYDRATION, CF_CALLBACK_VALIDATE_DATA_FLAG_NONE, cfapi/ CF_CALLBACK_VALIDATE_DATA_FLAG_EXPLICIT_HYDRATION, cfapi/CF_CALLBACK_VALIDATE_DATA_FLAGS, cfapi/CF_CALLBACK_VALIDATE_DATA_FLAG_NONE, cloudApi.cf_callback_validate_data_flags
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
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
 - CF_CALLBACK_VALIDATE_DATA_FLAGS
product: Windows
targetos: Windows
req.typenames: CF_CALLBACK_VALIDATE_DATA_FLAGS
req.redist: 
---

# CF_CALLBACK_VALIDATE_DATA_FLAGS enumeration


## -description


Flags to validate the data of a placeholder file or directory.


## -enum-fields




### -field CF_CALLBACK_VALIDATE_DATA_FLAG_NONE

No data validation flag.


### -field CF_CALLBACK_VALIDATE_DATA_FLAG_EXPLICIT_HYDRATION

<b>Note</b>  This value is new for Windows 10, version 1803.

Set if the callback is invoked as a result of a call to <a href="https://msdn.microsoft.com/4FFD7580-BF59-48D0-B6D7-516559914096">CfHydratePlaceholder</a>. 

