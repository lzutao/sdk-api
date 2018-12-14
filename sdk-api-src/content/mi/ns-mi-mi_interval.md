---
UID: NS:mi._MI_Interval
title: MI_Interval
author: windows-sdk-content
description: MI_Interval represents an interval of time.
old-location: wmi_v2\mi_interval.htm
tech.root: wmi_v2
ms.assetid: b6bf3d47-c292-4140-8bc6-f15ad8a8019f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MI_Interval, MI_Interval structure [Windows Management Infrastructure (MI)], mi/MI_Interval, wmi._mi_interval, wmi_v2.mi_interval
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: mi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8
req.target-min-winversvr: Windows Server 2012
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
 - Mi.h
api_name:
 - MI_Interval
product: Windows
targetos: Windows
req.typenames: MI_Interval
req.redist: Windows Management Framework 3.0 on Windows Server 2008 R2 with SP1, Windows 7 with SP1, and Windows Server 2008 with SP2
---

# MI_Interval structure


## -description


<b>MI_Interval</b> represents an interval of time.


## -struct-fields




### -field days

The number of days in the interval. (0-99999999)


### -field hours

The remaining number of hours in the interval. (0-23)


### -field minutes

The remaining number of minutes in the interval. (0-59)


### -field seconds

The remaining number of seconds in the interval. (0-59)


### -field microseconds

The remaining number of microseconds in the interval. (0-999999)


### -field __padding1

Reserved. The <b>MI_Interval</b> structure is padded to have the same size as <a href="https://msdn.microsoft.com/f06f1b0e-d21c-4b60-8099-222a1582fde1">MI_Timestamp</a>.


### -field __padding2

Reserved. The <b>MI_Interval</b> structure is padded to have the same size as <a href="https://msdn.microsoft.com/f06f1b0e-d21c-4b60-8099-222a1582fde1">MI_Timestamp</a>.


### -field __padding3

Reserved. The <b>MI_Interval</b> structure is padded to have the same size as <a href="https://msdn.microsoft.com/f06f1b0e-d21c-4b60-8099-222a1582fde1">MI_Timestamp</a>.
