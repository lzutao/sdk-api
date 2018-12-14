---
UID: NF:cfapi.CfGetCorrelationVector
title: CfGetCorrelationVector function
author: windows-sdk-content
description: Allows the sync provider to query the current correlation vector for a given placeholder file.
old-location: cloudapi\cfgetcorrelationvector.htm
tech.root: cfApi
ms.assetid: 3DB0AAFE-82DC-4707-8DB6-C52D4A9B2771
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CfGetCorrelationVector, CfGetCorrelationVector function, cfapi/CfGetCorrelationVector, cloudApi.cfgetcorrelationvector
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
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
req.lib: CldApi.lib
req.dll: CldApi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - CldApi.dll
api_name:
 - CfGetCorrelationVector
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CfGetCorrelationVector function


## -description


Allows the sync provider to query the current correlation vector for a given placeholder file.


## -parameters




### -param FileHandle [in]

The handle to the placeholder file.


### -param CorrelationVector [out]

The correlation vector for the <i>FileHandle</i>.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


