---
UID: NF:wbemdisp.ISWbemDateTime.get_MicrosecondsSpecified
title: ISWbemDateTime::get_MicrosecondsSpecified
author: windows-sdk-content
description: Boolean value that indicates whether the microseconds component in the CIM datetime value contains an interval or a wildcard value.
old-location: wmi\swbemdatetime_microsecondsspecified.htm
old-project: WmiSdk
ms.assetid: 65244ece-2326-4edc-b982-57e2046ec33e
ms.author: windowssdkdev
ms.date: 06/07/2018
ms.keywords: ISWbemDateTime interface [Windows Management Instrumentation],MicrosecondsSpecified property, ISWbemDateTime.get_MicrosecondsSpecified, ISWbemDateTime.put_MicrosecondsSpecified, ISWbemDateTime::get_MicrosecondsSpecified, MicrosecondsSpecified property [Windows Management Instrumentation], MicrosecondsSpecified property [Windows Management Instrumentation],ISWbemDateTime interface, MicrosecondsSpecified property [Windows Management Instrumentation],SWbemDateTime object, SWbemDateTime object [Windows Management Instrumentation],MicrosecondsSpecified property, SWbemDateTime.MicrosecondsSpecified, _hmm_swbemdatetime.microsecondsspecified, get_MicrosecondsSpecified, wmi.swbemdatetime_microsecondsspecified
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: wbemdisp.h
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
req.type-library: Wbemdisp.tlb
tech.root: 
req.typenames: WbemTimeout
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wbemdisp.dll
api_name:
 - SWbemDateTime.MicrosecondsSpecified
 - ISWbemDateTime.MicrosecondsSpecified
 - ISWbemDateTime.get_MicrosecondsSpecified
 - ISWbemDateTime.put_MicrosecondsSpecified
product: Windows
targetos: Windows
req.lib: 
req.dll: Wbemdisp.dll
req.irql: 
req.product: Windows Address Book 5.0
---

# ISWbemDateTime::get_MicrosecondsSpecified


## -description


The 
<b>MicrosecondsSpecified</b> property of the 
<a href="https://msdn.microsoft.com/3dd34c73-3c2b-4d59-827b-169cf8020213">SWbemDateTime</a> object is a Boolean value that indicates whether the microseconds component in the CIM datetime value contains an interval or a wildcard value. If 
<b>MicrosecondsSpecified</b> is <b>TRUE</b> and 
<a href="https://msdn.microsoft.com/ba5fcf17-7c26-4960-9da9-e380d90e5f3e">IsInterval</a> is <b>FALSE</b>, then 
<a href="https://msdn.microsoft.com/b810b781-86a3-4730-8114-44d10454f7c3">SWbemDateTime.Microseconds</a> contains a datetime value. A datetime value that contains an interval cannot be converted into either the <b>VT_DATE</b> format or the <b>FILETIME</b> format. If 
<a href="https://msdn.microsoft.com/55211da6-cbd5-4e61-ab7d-ee20363e9d81">HoursSpecified</a> is <b>FALSE</b> and 
<b>IsInterval</b> is <b>TRUE</b>, then <b>SWbemDateTime.Microseconds</b> contains an interval.

For an explanation of this syntax, see 
<a href="https://msdn.microsoft.com/889e6322-96f6-4a24-a084-e3b7bfa94a40">Document Conventions for the Scripting API</a>.

This property is read/write.


## -parameters


## -see-also




<a href="https://msdn.microsoft.com/2c18ef4d-4eb6-4c73-ad2e-31995b79e99d">DATETIME</a>



<a href="https://msdn.microsoft.com/3dd34c73-3c2b-4d59-827b-169cf8020213">SWbemDateTime</a>



<a href="https://msdn.microsoft.com/b810b781-86a3-4730-8114-44d10454f7c3">SWbemDateTime.Microseconds</a>
 

 
