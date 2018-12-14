---
UID: NF:cfapi.CfSetCorrelationVector
title: CfSetCorrelationVector function
author: windows-sdk-content
description: Allows a sync provider to instruct the platform to use a specific correlation vector for telemetry purposes on a placeholder file. This is optional.
old-location: cloudapi\cfsetcorrelationvector.htm
tech.root: cfApi
ms.assetid: B9B05D24-BEE5-4BE6-95D5-C28466D69543
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CfSetCorrelationVector, CfSetCorrelationVector function, cfapi/CfSetCorrelationVector, cloudApi.cfsetcorrelationvector
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
 - CfSetCorrelationVector
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CfSetCorrelationVector function


## -description


Allows a sync provider to instruct the platform to use a specific correlation vector for telemetry purposes on a placeholder file. This is optional.


## -parameters




### -param FileHandle [in]

The handle to the placeholder file.


### -param CorrelationVector [in]

A specific correlation vector to be associated with the <i>FileHandle</i>. 


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The platform automatically assigns a correlation vector to each file when it is first opened, and provides this correlation vector with each callback to the sync provider as part of the common <a href="https://msdn.microsoft.com/EF24E61E-4AF7-4946-A326-1F045267AE01">CF_CALLBACK_INFO</a>.  It is suggested that the sync engine call this function to increment the last digit of the correlation vector “clock” as the sync provider progresses through internal stages (as defined by the sync provider) of satisfying the request.


