---
UID: NF:faxcomex.IFaxOutgoingArchive.put_LowQuotaWaterMark
title: IFaxOutgoingArchive::put_LowQuotaWaterMark
author: windows-sdk-content
description: The IFaxOutgoingArchive::get_LowQuotaWaterMark property is a value that specifies the lower threshold for the archive of outbound fax messages, in megabytes.
old-location: fax\_mfax_faxoutgoingarchive_cpp_mfax_faxoutgoingarchive_lowquotawatermark_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_9nmz.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxOutgoingArchive interface [Fax Service],LowQuotaWaterMark property, IFaxOutgoingArchive.LowQuotaWaterMark, IFaxOutgoingArchive.get_LowQuotaWaterMark, IFaxOutgoingArchive.put_LowQuotaWaterMark, IFaxOutgoingArchive::LowQuotaWaterMark, IFaxOutgoingArchive::get_LowQuotaWaterMark, IFaxOutgoingArchive::put_LowQuotaWaterMark, LowQuotaWaterMark property [Fax Service], LowQuotaWaterMark property [Fax Service],IFaxOutgoingArchive interface, _mfax_faxoutgoingarchive.lowquotawatermark, fax._mfax_faxoutgoingarchive_cpp_mfax_faxoutgoingarchive_lowquotawatermark_cpp, fax._mfax_faxoutgoingarchive_lowquotawatermark, faxcomex/IFaxOutgoingArchive::LowQuotaWaterMark, faxcomex/IFaxOutgoingArchive::get_LowQuotaWaterMark, faxcomex/IFaxOutgoingArchive::put_LowQuotaWaterMark, put_LowQuotaWaterMark
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
 - IFaxOutgoingArchive.LowQuotaWaterMark
 - IFaxOutgoingArchive.get_LowQuotaWaterMark
 - IFaxOutgoingArchive.put_LowQuotaWaterMark
 - IFaxOutgoingArchive.get_LowQuotaWaterMark
 - IFaxOutgoingArchive.put_LowQuotaWaterMark
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxOutgoingArchive::put_LowQuotaWaterMark


## -description


The <b>IFaxOutgoingArchive::get_LowQuotaWaterMark</b> property is a value that specifies the lower threshold for the archive of outbound fax messages, in megabytes. If the fax service has issued a warning in the event log, the service does not issue additional warnings until the size of the outbound archive drops below this value. 

This property is read/write.


## -parameters


## -remarks



<div class="alert"><b>Note</b>  This property is not supported in Windows Vista, Windows Server 2008, and later versions of Windows. To access this property in Windows Vista, Windows Server 2008, and later versions of Windows,  get the <a href="https://msdn.microsoft.com/en-us/library/ms693549(v=VS.85).aspx">IFaxConfiguration</a> interface from the <a href="https://msdn.microsoft.com/en-us/library/Aa358976(v=VS.85).aspx">IFaxServer2</a> interface, and then call the  <a href="https://msdn.microsoft.com/en-us/library/Aa358924(v=VS.85).aspx">IFaxConfiguration::put_LowQuotaWaterMark</a>   or <a href="https://msdn.microsoft.com/en-us/library/Aa358924(v=VS.85).aspx">IFaxConfiguration::get_LowQuotaWaterMark</a> method.</div>
<div> </div>
To read this property, a user must have the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farQUERY_CONFIG</a> access right.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms688636(v=VS.85).aspx">IFaxOutgoingArchive</a>
 

 
