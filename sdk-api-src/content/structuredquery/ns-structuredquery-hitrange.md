---
UID: NS:structuredquery.tagHITRANGE
title: HITRANGE
author: windows-sdk-content
description: Identifies the range of matching data when query search conditions match indexed data.
old-location: search\_search_HITRANGE.htm
tech.root: search
ms.assetid: VS|SEARCH|~\search\wds3x\reference\structures\hitrange.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: HITRANGE, HITRANGE structure [search], _search_HITRANGE, search._search_HITRANGE, structuredquery/HITRANGE
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: structuredquery.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Structuredquery.idl
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
 - Structuredquery.h
api_name:
 - HITRANGE
product: Windows
targetos: Windows
req.typenames: HITRANGE
req.redist: 
---

# HITRANGE structure


## -description


Identifies the range of matching data when query search conditions match indexed data.


## -struct-fields




### -field iPosition

Type: <b>ULONG</b>

The beginning of the hit range.


### -field cLength

Type: <b>ULONG</b>

The length of the hit range.


## -remarks



The <b>HITRANGE</b> structure is useful for identifying where a search term matches the content from returned results, and for hit highlighting in user interfaces.


