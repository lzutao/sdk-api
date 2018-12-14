---
UID: NE:cfapi.CF_CALLBACK_DELETE_FLAGS
title: CF_CALLBACK_DELETE_FLAGS
author: windows-sdk-content
description: This callback is used to inform the sync provider that a placeholder file or directory under one of its sync roots is about to be deleted.
old-location: cloudapi\cf_callback_delete_flags.htm
tech.root: cfApi
ms.assetid: 76F9FB0C-F531-447F-8F0E-1EB849336771
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CF_CALLBACK_DELETE_FLAGS, CF_CALLBACK_DELETE_FLAGS enumeration, CF_CALLBACK_DELETE_FLAG_IS_DIRECTORY, CF_CALLBACK_DELETE_FLAG_NONE, cfapi/CF_CALLBACK_DELETE_FLAGS, cfapi/CF_CALLBACK_DELETE_FLAG_IS_DIRECTORY, cfapi/CF_CALLBACK_DELETE_FLAG_NONE, cloudApi.cf_callback_delete_flags
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
 - CF_CALLBACK_DELETE_FLAGS
product: Windows
targetos: Windows
req.typenames: CF_CALLBACK_DELETE_FLAGS
req.redist: 
---

# CF_CALLBACK_DELETE_FLAGS enumeration


## -description


This callback is used to inform the sync provider that a placeholder file or directory under one of its sync roots is about to be deleted.


## -enum-fields




### -field CF_CALLBACK_DELETE_FLAG_NONE

No delete flag.


### -field CF_CALLBACK_DELETE_FLAG_IS_DIRECTORY

The placeholder that is about to be deleted is a directory.
