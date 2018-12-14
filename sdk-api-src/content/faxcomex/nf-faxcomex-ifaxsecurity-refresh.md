---
UID: NF:faxcomex.IFaxSecurity.Refresh
title: IFaxSecurity::Refresh
author: windows-sdk-content
description: The IFaxSecurity::Refresh method refreshes FaxSecurity object information from the fax server.
old-location: fax\_mfax_faxsecurity_cpp_mfax_faxsecurity_refresh_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_9xrc.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxSecurity interface [Fax Service],Refresh method, IFaxSecurity.Refresh, IFaxSecurity::Refresh, Refresh, Refresh method [Fax Service], Refresh method [Fax Service],IFaxSecurity interface, _mfax_faxsecurity.refresh, fax._mfax_faxsecurity_cpp_mfax_faxsecurity_refresh_cpp, fax._mfax_faxsecurity_refresh, faxcomex/IFaxSecurity::Refresh
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
 - IFaxSecurity.Refresh
 - IFaxSecurity.Refresh
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxSecurity::Refresh


## -description


The <b>IFaxSecurity::Refresh</b> method refreshes <a href="https://msdn.microsoft.com/en-us/library/ms689509(v=VS.85).aspx">FaxSecurity</a> object information from the fax server.


## -parameters






## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



When the <b>IFaxSecurity::Refresh</b> method is called, any configuration changes made after the last <a href="https://msdn.microsoft.com/en-us/library/ms690247(v=VS.85).aspx">IFaxSecurity::Save</a> method call are lost.

To read this property, a user must have the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farQUERY_CONFIG</a> access right.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms689509(v=VS.85).aspx">FaxSecurity</a>



<a href="https://msdn.microsoft.com/en-us/library/ms689510(v=VS.85).aspx">IFaxSecurity</a>
 

 
