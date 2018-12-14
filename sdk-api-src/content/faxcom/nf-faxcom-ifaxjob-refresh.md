---
UID: NF:faxcom.IFaxJob.Refresh
title: IFaxJob::Refresh
author: windows-sdk-content
description: The IFaxJob::Refresh method updates FaxJob object information for the associated fax job.
old-location: fax\_mfax_ifaxjob_mfax_ifaxjob_refresh_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_7bqg.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxJob interface [Fax Service],Refresh method, IFaxJob.Refresh, IFaxJob::Refresh, Refresh, Refresh method [Fax Service], Refresh method [Fax Service],IFaxJob interface, _mfax_ifaxjob_refresh, fax._mfax_ifaxjob_mfax_ifaxjob_refresh_cpp, fax._mfax_ifaxjob_refresh, faxcom/IFaxJob::Refresh
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
req.dll: Faxcom.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Faxcom.dll
api_name:
 - IFaxJob.Refresh
 - IFaxJob.Refresh
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxJob::Refresh


## -description


The <b>IFaxJob::Refresh</b> method updates <a href="https://msdn.microsoft.com/en-us/library/ms692342(v=VS.85).aspx">FaxJob</a> object information for the associated fax job.


## -parameters






## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Call the <b>IFaxJob::Refresh</b> method to poll the fax service for new information about a specified fax job. After you successfully call <b>IFaxJob::Refresh</b>, you must call the appropriate <a href="https://msdn.microsoft.com/en-us/library/ms692310(v=VS.85).aspx">IFaxJob</a> interface method to retrieve new attribute values that are valid.

It is recommended that you limit calls to this method because frequent calls to <b>IFaxJob::Refresh</b> can degrade system performance.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms691931(v=VS.85).aspx">Fax Service Client API Interfaces</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692829(v=VS.85).aspx">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692310(v=VS.85).aspx">IFaxJob</a>



<a href="https://msdn.microsoft.com/en-us/library/ms692372(v=VS.85).aspx">IFaxJobs</a>
 

 
