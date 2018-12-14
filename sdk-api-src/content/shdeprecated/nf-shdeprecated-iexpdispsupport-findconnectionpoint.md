---
UID: NF:shdeprecated.IExpDispSupport.FindConnectionPoint
title: IExpDispSupport::FindConnectionPoint
author: windows-sdk-content
description: Deprecated. Gets connection points for browser events.
old-location: shell\IExpDispSupport_FindCIE4ConnectionPoint.htm
tech.root: shell
ms.assetid: ef8d4e8c-7f85-4920-b149-1bf277d3fd5e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DIID_DWebBrowserEvents, DIID_DWebBrowserEvents2, FindConnectionPoint, FindConnectionPoint method [Windows Shell], FindConnectionPoint method [Windows Shell],IExpDispSupport interface, IExpDispSupport interface [Windows Shell],FindConnectionPoint method, IExpDispSupport.FindConnectionPoint, IExpDispSupport::FindConnectionPoint, IID_IPropertyNotifySink, shdeprecated/IExpDispSupport::FindConnectionPoint, shell.IExpDispSupport_FindCIE4ConnectionPoint, zone_IExpDispSupport_FindCIE4ConnectionPoint
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shdeprecated.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shdeprecated.idl
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
 - COM
api_location:
 - Shdeprecated.h
api_name:
 - IExpDispSupport.FindConnectionPoint
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: Internet Explorer 4.0
---

# IExpDispSupport::FindConnectionPoint


## -description


Deprecated. Gets connection points for browser events.


## -parameters




### -param riid [in]

Type: <b>REFIID</b>

The IID of the interface on the connection point container whose connection point object is being requested. One of the following values.



#### DIID_DWebBrowserEvents

Value that indicates a member of the <a href="https://msdn.microsoft.com/5acfc998-2c97-462e-ab16-fd9acfb6e9c3">DWebBrowserEvents</a> interface.



#### DIID_DWebBrowserEvents2

Value that indicates a member of the <a href="https://msdn.microsoft.com/0286e985-5403-41c5-bc24-12b537b8ba0e">DWebBrowserEvents2</a> interface.



#### IID_IPropertyNotifySink

Value that indicates a member of the <a href="https://msdn.microsoft.com/bfdf315c-6375-4c77-abd8-03f07342820f">IPropertyNotifySink</a> interface.


### -param ppccp [out]

Type: <b>CIE4ConnectionPoint**</b>

The address of a pointer to the browser connection point.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



<b>IExpDispSupport::FindCIE4ConnectionPoint</b> was created specifically for use with Windows Internet Explorer 4.0.


