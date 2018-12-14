---
UID: NF:cfapi.CfGetSyncRootInfoByPath
title: CfGetSyncRootInfoByPath function
author: windows-sdk-content
description: Gets various sync root information given a file under the sync root.
old-location: cloudapi\cfgetsyncrootinfobypath.htm
tech.root: cfApi
ms.assetid: 0FEEF910-3545-4D94-BFF9-88AEE084F454
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CfGetSyncRootInfoByPath, CfGetSyncRootInfoByPath function, cfapi/CfGetSyncRootInfoByPath, cloudApi.cfgetsyncrootinfobypath
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
 - CfGetSyncRootInfoByPath
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CfGetSyncRootInfoByPath function


## -description


Gets various sync root information given a file under the sync root.


## -parameters




### -param FilePath [in]

A fully qualified path to a file whose sync root information is to be queried


### -param InfoClass [in]

Types of sync root information.


### -param InfoBuffer [out]

A pointer to a buffer that will receive the sync root information.


### -param InfoBufferLength [in]

Length, in bytes, of the <i>InfoBuffer</i>.


### -param ReturnedLength [out, optional]

Length, in bytes, of the returned sync root information. Refer to <a href="https://msdn.microsoft.com/FAD56873-8812-42DC-9975-9507F73BD9E3">CfRegisterSyncRoot</a> for details about the sync root information.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


