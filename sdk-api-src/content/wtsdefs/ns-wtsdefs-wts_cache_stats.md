---
UID: NS:wtsdefs._WTS_CACHE_STATS
title: WTS_CACHE_STATS
author: windows-sdk-content
description: Contains protocol cache statistics.
old-location: termserv\wts_cache_stats.htm
tech.root: TermServ
ms.assetid: 3c29596f-77c6-415b-bf97-529f70b9d9fe
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PWTS_CACHE_STATS, 1, 2, 3, PWRDS_CACHE_STATS, PWRDS_CACHE_STATS structure pointer [Remote Desktop Services], PWTS_CACHE_STATS, PWTS_CACHE_STATS structure pointer [Remote Desktop Services], WRDS_CACHE_STATS, WRDS_CACHE_STATS structure [Remote Desktop Services], WTS_CACHE_STATS, WTS_CACHE_STATS structure [Remote Desktop Services], termserv.wts_cache_stats, wtsdefs/PWRDS_CACHE_STATS, wtsdefs/PWTS_CACHE_STATS, wtsdefs/WRDS_CACHE_STATS, wtsdefs/WTS_CACHE_STATS"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: wtsdefs.h
req.include-header: Wtsprotocol.h
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2
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
 - Wtsdefs.h
api_name:
 - WTS_CACHE_STATS
product: Windows
targetos: Windows
req.typenames: WTS_CACHE_STATS, *PWTS_CACHE_STATS
req.redist: 
---

# WTS_CACHE_STATS structure


## -description


Contains protocol cache statistics.


## -struct-fields




### -field Specific

An integer index that specifies the <a href="https://msdn.microsoft.com/e6abb47e-248b-482d-9206-936092c391ce">WTS_CACHE_STATS_UN</a> union member that contains the cache data. This can be one of the following values.



#### 1

The cache data is contained in the <b>ProtocolCache</b> member.



#### 2

The cache data is contained in the <b>TShareCacheStats</b> member.



#### 3

The cache data is contained in the <b>Reserved</b> member.


### -field Data

A <a href="https://msdn.microsoft.com/e6abb47e-248b-482d-9206-936092c391ce">WTS_CACHE_STATS_UN</a> union that contains the cache statistics.


### -field Data.switch_is

 


### -field Data.switch_is.Specific

 


### -field ProtocolType

An integer that specifies the protocol type. This is not currently used by the Remote Desktop Services service.


### -field Length

An integer that contains the length of the data in the <b>Reserved</b> member of the <a href="https://msdn.microsoft.com/e6abb47e-248b-482d-9206-936092c391ce">WTS_CACHE_STATS_UN</a> union. The maximum size is WTS_MAX_CACHE_RESERVED multiplied by the length of an unsigned long integer.


## -remarks



This structure is a member of the <a href="https://msdn.microsoft.com/20e66033-fc79-49c9-af0e-abaf6e4ba501">WTS_PROTOCOL_STATUS</a> structure.


