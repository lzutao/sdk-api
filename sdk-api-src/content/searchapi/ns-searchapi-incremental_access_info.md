---
UID: NS:searchapi._INCREMENTAL_ACCESS_INFO
title: INCREMENTAL_ACCESS_INFO
author: windows-sdk-content
description: Contains access information used by an incremental crawl, such as the last access date and modification time.
old-location: search\_search_INCREMENTAL_ACCESS_INFO.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\structures\incremental_access_info.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: INCREMENTAL_ACCESS_INFO, INCREMENTAL_ACCESS_INFO structure [search], _search_INCREMENTAL_ACCESS_INFO, search._search_INCREMENTAL_ACCESS_INFO, searchapi/INCREMENTAL_ACCESS_INFO
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: searchapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Srchprth.idl
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
 - Searchapi.h
api_name:
 - INCREMENTAL_ACCESS_INFO
product: Windows
targetos: Windows
req.typenames: INCREMENTAL_ACCESS_INFO
req.redist: Windows Desktop Search (WDS) 3.0
---

# INCREMENTAL_ACCESS_INFO structure


## -description


Contains access information used by an incremental crawl, such as the last access date and modification time. 


## -struct-fields




### -field dwSize

Type: <b>DWORD</b>

Size of the file in bytes.


### -field ftLastModifiedTime

Type: <b><a href="_com_FILETIME">FILETIME</a></b>

Last time the file was modified.
