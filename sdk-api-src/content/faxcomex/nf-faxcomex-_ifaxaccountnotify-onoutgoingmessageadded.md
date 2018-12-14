---
UID: NF:faxcomex._IFaxAccountNotify.OnOutgoingMessageAdded
title: "_IFaxAccountNotify::OnOutgoingMessageAdded"
author: windows-sdk-content
description: The fax service calls the IFaxAccountNotify::OnOutgoingMessageAdded method when an outgoing message is added to the outbound fax archive.
old-location: fax\_mfax_ifaxaccountnotify_onoutgoingmessageadded.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\reference\serviceextendedcom\i\ifaxaccountnotify\onoutgoingmessageadded.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxAccountNotify.OnOutgoingMessageAdded, OnOutgoingMessageAdded, OnOutgoingMessageAdded method [Fax Service], OnOutgoingMessageAdded method [Fax Service],_IFaxAccountNotify interface, _IFaxAccountNotify interface [Fax Service],OnOutgoingMessageAdded method, _IFaxAccountNotify.OnOutgoingMessageAdded, _IFaxAccountNotify::OnOutgoingMessageAdded, _mfax_ifaxaccountnotify_onoutgoingmessageadded, fax._mfax_ifaxaccountnotify_onoutgoingmessageadded, faxcomex/_IFaxAccountNotify::OnOutgoingMessageAdded
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
 - _IFaxAccountNotify.OnOutgoingMessageAdded
 - IFaxAccountNotify.OnOutgoingMessageAdded
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# _IFaxAccountNotify::OnOutgoingMessageAdded


## -description


The fax service calls the <b>IFaxAccountNotify::OnOutgoingMessageAdded</b> method when an outgoing message is added to the outbound fax archive.


## -parameters




### -param pFaxAccount [in]

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Aa359058(v=VS.85).aspx">IFaxAccount</a>*</b>

A <a href="https://msdn.microsoft.com/en-us/library/Aa359058(v=VS.85).aspx">IFaxAccount</a> object.


### -param bstrMessageId [in]

Type: <b>BSTR</b>

Null-terminated string that contains the ID of the message added to the outbound fax archive.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To implement this functionality in Visual Basic, select and implement the appropriate event procedure.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa359031(v=VS.85).aspx">IFaxAccountNotify</a>
 

 
