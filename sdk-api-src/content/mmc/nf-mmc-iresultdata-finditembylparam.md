---
UID: NF:mmc.IResultData.FindItemByLParam
title: IResultData::FindItemByLParam
author: windows-sdk-content
description: The IResultData::FindItemByLParam method enables the snap-in to find an item or subitem based on its user-inserted lParam value.
old-location: mmc\iresultdata_finditembylparam.htm
tech.root: mmc
ms.assetid: f26be5d5-9b7d-4cbd-b70c-431799c68e5e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FindItemByLParam, FindItemByLParam method [MMC], FindItemByLParam method [MMC],IResultData interface, FindItemByLParam method [MMC],IResultData2 interface, IResultData interface [MMC],FindItemByLParam method, IResultData.FindItemByLParam, IResultData2 interface [MMC],FindItemByLParam method, IResultData2::FindItemByLParam, IResultData::FindItemByLParam, _slate_iresultdata_finditembylparam, mmc.iresultdata_finditembylparam, mmc/IResultData2::FindItemByLParam, mmc/IResultData::FindItemByLParam
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mmc.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: Mmcndmgr.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Mmcndmgr.dll
api_name:
 - IResultData.FindItemByLParam
 - IResultData2.FindItemByLParam
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IResultData::FindItemByLParam


## -description


The <b>IResultData::FindItemByLParam</b> method enables the snap-in to find an item or subitem based on its user-inserted lParam value.


## -parameters




### -param lParam [in]

A generic 32-bit value in which information can be stored.


### -param pItemID [out]

A pointer to an item identifier to hold the results of the search for the lParam value.


## -returns



This method can return one of these values.




## -remarks



FindItemByLParam searches for an item based on its lParam. The unique identifier (cookie) of the first item in the list with a matching lParam is returned in pItemID. If no item is found, the search returns S_FALSE.

This method does not support virtual lists.




## -see-also




<a href="https://msdn.microsoft.com/58f8bcdb-b062-4048-92fc-eb652ce62c5b">IResultData</a>



<a href="https://msdn.microsoft.com/cca0c2a4-7a41-48d1-bdaa-27b7aad7cc05">IResultData2</a>
 

 
