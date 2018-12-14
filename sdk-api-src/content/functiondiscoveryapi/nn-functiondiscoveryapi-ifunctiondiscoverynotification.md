---
UID: NN:functiondiscoveryapi.IFunctionDiscoveryNotification
title: IFunctionDiscoveryNotification
author: windows-sdk-content
description: This interface is implemented by the client program to support asynchronous queries and is called by Function Discovery to notify the client program when a function instance that meets the query parameters has been added or removed.
old-location: ncd\ifunctiondiscoverynotification.htm
tech.root: fundisc
ms.assetid: 1819fe08-b151-482d-8e2c-1d599fd15609
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFunctionDiscoveryNotification, IFunctionDiscoveryNotification interface, IFunctionDiscoveryNotification interface,described, functiondiscoveryapi/IFunctionDiscoveryNotification, ncd.ifunctiondiscoverynotification
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: functiondiscoveryapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: FunctionDiscoveryAPI.idl
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
 - functiondiscoveryapi.h
api_name:
 - IFunctionDiscoveryNotification
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFunctionDiscoveryNotification interface


## -description


<p class="CCE_Message">[Function Discovery is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions.]

This interface is implemented by the client program  to support asynchronous queries and is called by Function Discovery to notify the client program when a function instance that meets the query parameters has been added or removed.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IFunctionDiscoveryNotification</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IFunctionDiscoveryNotification</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IFunctionDiscoveryNotification</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c4dcc4e9-7acf-44d3-b337-1ac01afa19b0">OnError</a>
</td>
<td align="left" width="63%">
Receives errors that occur during asynchronous query processing.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/4ebfdf15-ca37-4905-b842-8854a0bd276b">OnEvent</a>
</td>
<td align="left" width="63%">
Receives any add, remove, or update events.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ab4d0fc6-de3f-49cf-b53c-573222a8bc89">OnUpdate</a>
</td>
<td align="left" width="63%">
Indicates that a function instance has been added, removed, or changed.

</td>
</tr>
</table> 


## -remarks



This interface must be implemented by the client program in order to receive notifications from Function Discovery. The address of the client program's implementation is passed to one of the query methods to enable notifications for function instances which meet the query parameters.

 Function Discovery calls the client program's <a href="https://msdn.microsoft.com/ab4d0fc6-de3f-49cf-b53c-573222a8bc89">IFunctionDiscoveryNotification::OnUpdate</a> method to perform the actual notification, which is generated for a function instance when it is added or removed. <div class="alert"><b>Note</b>  Some Function discovery providers will also generate a notification when a function instance is modified by changing a category or one or more properties assigned to it.</div>
<div> </div>



#### Examples

The examples that appear on individual method pages are based on the following class declaration.

<pre class="syntax" xml:space="preserve"><code>class CMyNotificationListener : public CFunctionDiscoveryNotificationWrapper
{
public:
    CMyNotificationListener() {
        m_hAddEvent      = CreateEvent( NULL, FALSE, FALSE, NULL );
        m_hRemoveEvent   = CreateEvent( NULL, FALSE, FALSE, NULL );
        m_hChangeEvent   = CreateEvent( NULL, FALSE, FALSE, NULL );
    }

    ~CMyNotificationListener() {
        CloseHandle( m_hAddEvent );
        CloseHandle( m_hRemoveEvent );
        CloseHandle( m_hChangeEvent );
    }
        

private:
    HANDLE m_hAddEvent, m_hRemoveEvent, m_hChangeEvent;
};
</code></pre>

