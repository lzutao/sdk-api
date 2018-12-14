---
UID: NF:faxcomex._IFaxServerNotify2.OnNewCall
title: "_IFaxServerNotify2::OnNewCall"
author: windows-sdk-content
description: The fax service calls the IFaxServerNotify2::OnNewCall method when there is a new incoming fax call.
old-location: fax\_mfax_ifaxservernotify2_onnewcall.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_onnewcall.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxServerNotify2 interface [Fax Service],OnNewCall method, IFaxServerNotify2.OnNewCall, IFaxServerNotify2::OnNewCall, OnNewCall, OnNewCall method [Fax Service], OnNewCall method [Fax Service],IFaxServerNotify2 interface, _IFaxServerNotify2.OnNewCall, _IFaxServerNotify2::OnNewCall, _mfax_ifaxservernotify2_onnewcall, fax._mfax_ifaxservernotify2_onnewcall, faxcomex/IFaxServerNotify2::OnNewCall
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcomex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - IFaxServerNotify2.OnNewCall
 - IFaxServerNotify2.OnNewCall
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# _IFaxServerNotify2::OnNewCall


## -description


The fax service calls the <b>IFaxServerNotify2::OnNewCall</b> method when there is a new incoming fax call.


## -parameters




### -param pFaxServer

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa358976(v=VS.85).aspx">IFaxServer2</a>*</b>

A <a href="https://msdn.microsoft.com/en-us/library/Aa358976(v=VS.85).aspx">IFaxServer2</a> object.


### -param lCallId

Type: <b>long</b>

Long value that specifies the call's ID.


### -param lDeviceId

Type: <b>long</b>

Long value that specifies the device ID of the device receiving the new incoming fax call.


### -param bstrCallerId

Type: <b>long</b>

Null-terminated string that identifies the calling device for the new incoming fax call.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To implement this functionality in Visual Basic, select and implement the appropriate event procedure. For an example, see <a href="https://msdn.microsoft.com/en-us/library/ms693013(v=VS.85).aspx">Registering for Fax Events</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa358971(v=VS.85).aspx">IFaxServerNotify2</a>
 

 
