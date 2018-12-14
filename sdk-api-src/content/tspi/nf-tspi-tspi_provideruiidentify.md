---
UID: NF:tspi.TSPI_providerUIIdentify
title: TSPI_providerUIIdentify function
author: windows-sdk-content
description: The TSPI_providerUIIdentify function extracts from the service provider the fully qualified path to load the service provider's UI DLL component.
old-location: tspi\tspi_provideruiidentify.htm
tech.root: tapi
ms.assetid: 4ff4b695-8947-4ece-998c-6b443025c2d9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TSPI_providerUIIdentify, TSPI_providerUIIdentify function [TAPI 2.2], _tspi_tspi_provideruiidentify, tspi.tspi_provideruiidentify, tspi/TSPI_providerUIIdentify
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: tspi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - UserDefined
api_location:
 - Tspi.h
api_name:
 - TSPI_providerUIIdentify
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TSPI_providerUIIdentify function


## -description


The 
<b>TSPI_providerUIIdentify</b> function extracts from the service provider the fully qualified path to load the service provider's UI DLL component.

Implementation is mandatory if the service provider implements any UI DLL functions.


## -parameters




### -param lpszUIDLLName

Pointer to a block of memory at least MAX_PATH in length, into which the service provider must copy a null-terminated string specifying the fully qualified path for the DLL containing the service provider functions which must execute in the process of the calling application.


## -returns



Returns zero if successful. Shouldn't ever fail, but if it does returns one of these negative error values:

LINEERR_NOMEM, LINEERR_OPERATIONFAILED.


