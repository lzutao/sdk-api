---
UID: NF:faxcomex.IFaxIncomingJob.get_ExtendedStatus
title: IFaxIncomingJob::get_ExtendedStatus
author: windows-sdk-content
description: The ExtendedStatus property is a null-terminated string that describes the job's extended status.
old-location: fax\_mfax_faxincomingjob_cpp_mfax_faxincomingjob_extendedstatus_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_7v03.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ExtendedStatus property [Fax Service], ExtendedStatus property [Fax Service],IFaxIncomingJob interface, IFaxIncomingJob interface [Fax Service],ExtendedStatus property, IFaxIncomingJob.ExtendedStatus, IFaxIncomingJob.get_ExtendedStatus, IFaxIncomingJob::ExtendedStatus, IFaxIncomingJob::get_ExtendedStatus, _mfax_faxincomingjob.extendedstatus, fax._mfax_faxincomingjob_cpp_mfax_faxincomingjob_extendedstatus_cpp, fax._mfax_faxincomingjob_extendedstatus, faxcomex/IFaxIncomingJob::ExtendedStatus, faxcomex/IFaxIncomingJob::get_ExtendedStatus, get_ExtendedStatus
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
 - IFaxIncomingJob.ExtendedStatus
 - IFaxIncomingJob.get_ExtendedStatus
 - IFaxIncomingJob.get_ExtendedStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxIncomingJob::get_ExtendedStatus


## -description


The <b>ExtendedStatus</b> property is a null-terminated string that describes the job's extended status.

This property is read-only.


## -parameters


## -remarks



The <b>ExtendedStatus</b> property can have a value only if the fax service provider (FSP) returns a proprietary status code in the <a href="https://msdn.microsoft.com/en-us/library/ms686029(v=VS.85).aspx">ExtendedStatusCode</a> property. Otherwise, the <b>ExtendedStatus</b> property will contain an empty string.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms684876(v=VS.85).aspx">FaxIncomingJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms684878(v=VS.85).aspx">IFaxIncomingJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692952(v=VS.85).aspx">Visual Basic Example</a>
 

 
