---
UID: NF:faxcomex.IFaxDocument.get_ScheduleTime
title: IFaxDocument::get_ScheduleTime
author: windows-sdk-content
description: The IFaxDocument::get_ScheduleTime property indicates the time to submit the fax for processing to the fax service.
old-location: fax\_mfax_faxdocument_cpp_mfax_faxdocument_scheduletime_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_459h.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxDocument interface [Fax Service],ScheduleTime property, IFaxDocument.ScheduleTime, IFaxDocument.get_ScheduleTime, IFaxDocument.put_ScheduleTime, IFaxDocument::ScheduleTime, IFaxDocument::get_ScheduleTime, IFaxDocument::put_ScheduleTime, ScheduleTime property [Fax Service], ScheduleTime property [Fax Service],IFaxDocument interface, _mfax_faxdocument.scheduletime, fax._mfax_faxdocument_cpp_mfax_faxdocument_scheduletime_cpp, fax._mfax_faxdocument_scheduletime, faxcomex/IFaxDocument::ScheduleTime, faxcomex/IFaxDocument::get_ScheduleTime, faxcomex/IFaxDocument::put_ScheduleTime, get_ScheduleTime
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcomex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fxscomex.dll
api_name:
 - IFaxDocument.ScheduleTime
 - IFaxDocument.get_ScheduleTime
 - IFaxDocument.put_ScheduleTime
 - IFaxDocument.get_ScheduleTime
 - IFaxDocument.put_ScheduleTime
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxDocument::get_ScheduleTime


## -description


The <b>IFaxDocument::get_ScheduleTime</b> property indicates the time to submit the fax for processing to the fax service.

This property is read/write.


## -parameters


## -remarks



If the time specified has passed, the fax service sends the fax as soon as a device is available. By default, <b>IFaxDocument::get_ScheduleTime</b> is set to zero, meaning that no time is specified.

Note that the fax service ignores this parameter unless you set the <a href="https://msdn.microsoft.com/en-us/library/ms686190(v=VS.85).aspx">IFaxDocument::get_ScheduleType</a> property to <a href="https://msdn.microsoft.com/en-us/library/ms689199(v=VS.85).aspx">fstSpecific_TIME</a>.

<div class="alert"><b>Note</b>  The value of the <b>IFaxDocument::get_ScheduleTime</b> property must include the date and time for submitting the fax.</div>
<div> </div>



## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms685958(v=VS.85).aspx">FaxDocument</a>



<a href="https://msdn.microsoft.com/en-us/library/ms685960(v=VS.85).aspx">IFaxDocument</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692936(v=VS.85).aspx">Visual Basic Example</a>
 

 
