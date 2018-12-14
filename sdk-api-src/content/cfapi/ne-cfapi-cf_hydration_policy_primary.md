---
UID: NE:cfapi.CF_HYDRATION_POLICY_PRIMARY
title: CF_HYDRATION_POLICY_PRIMARY
author: windows-sdk-content
description: Allows a sync provider to control how placeholder files should be hydrated by the platform. This is the primary policy.
old-location: cloudapi\cf_hydration_policy_primary.htm
tech.root: cfApi
ms.assetid: 47ACA107-80AA-42B3-B583-399323E2B11C
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CF_HYDRATION_POLICY_ALWAYS_FULL, CF_HYDRATION_POLICY_FULL, CF_HYDRATION_POLICY_PARTIAL, CF_HYDRATION_POLICY_PRIMARY, CF_HYDRATION_POLICY_PRIMARY enumeration, CF_HYDRATION_POLICY_PROGRESSIVE, cfapi/CF_HYDRATION_POLICY_ALWAYS_FULL, cfapi/CF_HYDRATION_POLICY_FULL, cfapi/CF_HYDRATION_POLICY_PARTIAL, cfapi/CF_HYDRATION_POLICY_PRIMARY, cfapi/CF_HYDRATION_POLICY_PROGRESSIVE, cloudApi.cf_hydration_policy_primary
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
 - CF_HYDRATION_POLICY_PRIMARY
product: Windows
targetos: Windows
req.typenames: CF_HYDRATION_POLICY_PRIMARY
req.redist: 
---

# CF_HYDRATION_POLICY_PRIMARY enumeration


## -description


Allows a sync provider to control how placeholder files should be hydrated by the platform. This is the primary policy.


## -enum-fields




### -field CF_HYDRATION_POLICY_PARTIAL

The same behavior as <b>CF_HYDRATION_POLICY_PROGRESSIVE</b>, except that <b>CF_HYDRATION_POLICY_PARTIAL</b> does not have continuous hydration in the background.


### -field CF_HYDRATION_POLICY_PROGRESSIVE

When <b>CF_HYDRATION_POLICY_PROGRESSIVE</b> is selected, the platform will allow a placeholder to be dehydrated. When the platform detects access to a dehydrated placeholder, it will complete the user IO request as soon as it determines that sufficient data is received from the sync provider. However, the platform will continue requesting the remaining content in the placeholder from the sync provider in the background until either the full content of the placeholder is available locally, or the last user handle on the placeholder is closed.

<div class="alert"><b>Note</b>  <p class="note">Sync providers who opt in for <b>CF_HYDRATION_POLICY_PROGRESSIVE</b> may not assume that hydration callbacks arrive sequentially from offset 0. In other words, sync providers with <b>CF_HYDRATION_POLICY_PROGRESSIVE</b> policy are expected to handle random seeks on the placeholder.

</div>
<div> </div>

### -field CF_HYDRATION_POLICY_FULL

When <b>CF_HYDRATION_POLICY_FULL</b> is selected, the platform will allow a placeholder to be dehydrated. When the platform detects access to a dehydrated placeholder, it will ensure that the full content of the placeholder is available locally before completing the user IO request, even if the request is only asking for 1 byte.


### -field CF_HYDRATION_POLICY_ALWAYS_FULL

When <b>CF_HYDRATION_POLICY_ALWAYS_FULL</b> is selected, the platform will block any placeholder operation that could result in a not fully hydrated placeholder, which includes <a href="https://msdn.microsoft.com/96A6F62E-7F14-40B5-AB57-260DC9B1DF89">CfCreatePlaceholders</a>, <a href="https://msdn.microsoft.com/13F2BF9A-505F-4CFB-B008-7DDE85A3C581">CfUpdatePlaceholder</a> with the dehydrate option, and <a href="https://msdn.microsoft.com/FDDE9CB0-E1A2-46D6-94E0-228495675271">CfConvertToPlaceholder</a> with the dehydrate option.
