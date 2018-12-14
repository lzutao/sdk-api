---
UID: NF:faxcomex._IFaxServerNotify2.OnIncomingMessageAdded
title: "_IFaxServerNotify2::OnIncomingMessageAdded"
author: windows-sdk-content
description: The fax service calls the IFaxServerNotify2::OnIncomingMessageAdded method when an incoming message is added to the inbound fax archive.
old-location: fax\_mfax_ifaxservernotify2_onincomingmessageadded.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_onincomingmessageadded.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxServerNotify2 interface [Fax Service],OnIncomingMessageAdded method, IFaxServerNotify2.OnIncomingMessageAdded, IFaxServerNotify2::OnIncomingMessageAdded, OnIncomingMessageAdded, OnIncomingMessageAdded method [Fax Service], OnIncomingMessageAdded method [Fax Service],IFaxServerNotify2 interface, _IFaxServerNotify2.OnIncomingMessageAdded, _IFaxServerNotify2::OnIncomingMessageAdded, _mfax_ifaxservernotify2_onincomingmessageadded, fax._mfax_ifaxservernotify2_onincomingmessageadded, faxcomex/IFaxServerNotify2::OnIncomingMessageAdded
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
 - IFaxServerNotify2.OnIncomingMessageAdded
 - IFaxServerNotify2.OnIncomingMessageAdded
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# _IFaxServerNotify2::OnIncomingMessageAdded


## -description


The fax service calls the <b>IFaxServerNotify2::OnIncomingMessageAdded</b> method when an incoming message is added to the inbound fax archive.


## -parameters




### -param pFaxServer

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa358976(v=VS.85).aspx">IFaxServer2</a>*</b>

A <a href="https://msdn.microsoft.com/en-us/library/Aa358976(v=VS.85).aspx">IFaxServer2</a> object.


### -param bstrMessageId

Type: <b>BSTR</b>

Null-terminated string that contains the ID of the message added to the inbound fax archive.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To implement this functionality in Visual Basic, select and implement the appropriate event procedure. For an example, see <a href="https://msdn.microsoft.com/en-us/library/ms693013(v=VS.85).aspx">Registering for Fax Events</a>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa358971(v=VS.85).aspx">IFaxServerNotify2</a>
 

 
