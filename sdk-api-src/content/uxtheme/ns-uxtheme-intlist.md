---
UID: NS:uxtheme._INTLIST
title: INTLIST
author: windows-sdk-content
description: Contains an array or list of int data items from a visual style.
old-location: controls\INTLIST.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\userex\structures\intlist.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PINTLIST, INTLIST, INTLIST structure [Windows Controls], PINTLIST, PINTLIST structure pointer [Windows Controls], controls.INTLIST, controls.inet_INTLIST, inet_INTLIST, inet_INTLIST_cpp, uxtheme/INTLIST, uxtheme/PINTLIST"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: uxtheme.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - UxTheme.h
api_name:
 - INTLIST
product: Windows
targetos: Windows
req.typenames: INTLIST, *PINTLIST
req.redist: 
---

# INTLIST structure


## -description


Contains an array or list of <b>int</b> data items from a visual style.


## -struct-fields




### -field iValueCount

Type: <b>int</b>

Number of values in the list.


### -field iValues

Type: <b>int[MAX_INTLIST_COUNT]</b>

List of integers. The constant MAX_INTLIST_COUNT, by definition, is equal to 402 under Windows Vista, but only 10 under earlier versions of Windows.


## -remarks



The lists are returned by <a href="https://msdn.microsoft.com/123ddb53-4447-4b6b-a311-61da47090e94">GetThemeIntList</a>.


