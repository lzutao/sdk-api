---
UID: NF:xenroll.ICEnroll.get_RequestStoreFlags
title: ICEnroll::get_RequestStoreFlags
author: windows-sdk-content
description: Sets or retrieves the registry location used for the request store.
old-location: security\icenroll4_requeststoreflags.htm
tech.root: seccrypto
ms.assetid: 399870f0-69e1-4a21-a7fa-c3de9ee66876
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CEnroll object [Security],RequestStoreFlags property, ICEnroll interface [Security],RequestStoreFlags property, ICEnroll.RequestStoreFlags, ICEnroll.get_RequestStoreFlags, ICEnroll2 interface [Security],RequestStoreFlags property, ICEnroll2.RequestStoreFlags, ICEnroll2::get_RequestStoreFlags, ICEnroll2::put_RequestStoreFlags, ICEnroll3 interface [Security],RequestStoreFlags property, ICEnroll3.RequestStoreFlags, ICEnroll3::get_RequestStoreFlags, ICEnroll3::put_RequestStoreFlags, ICEnroll4 interface [Security],RequestStoreFlags property, ICEnroll4.RequestStoreFlags, ICEnroll4::RequestStoreFlags, ICEnroll4::get_RequestStoreFlags, ICEnroll4::put_RequestStoreFlags, ICEnroll::get_RequestStoreFlags, ICEnroll::put_RequestStoreFlags, RequestStoreFlags property [Security], RequestStoreFlags property [Security],CEnroll object, RequestStoreFlags property [Security],ICEnroll interface, RequestStoreFlags property [Security],ICEnroll2 interface, RequestStoreFlags property [Security],ICEnroll3 interface, RequestStoreFlags property [Security],ICEnroll4 interface, get_RequestStoreFlags, security.icenroll4_requeststoreflags, xenroll/ICEnroll2::RequestStoreFlags, xenroll/ICEnroll2::get_RequestStoreFlags, xenroll/ICEnroll2::put_RequestStoreFlags, xenroll/ICEnroll3::RequestStoreFlags, xenroll/ICEnroll3::get_RequestStoreFlags, xenroll/ICEnroll3::put_RequestStoreFlags, xenroll/ICEnroll4::RequestStoreFlags, xenroll/ICEnroll4::get_RequestStoreFlags, xenroll/ICEnroll4::put_RequestStoreFlags, xenroll/ICEnroll::RequestStoreFlags, xenroll/ICEnroll::get_RequestStoreFlags, xenroll/ICEnroll::put_RequestStoreFlags
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: xenroll.h
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
req.lib: Uuid.lib
req.dll: Xenroll.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Xenroll.dll
api_name:
 - ICEnroll4.RequestStoreFlags
 - ICEnroll4.get_RequestStoreFlags
 - ICEnroll4.put_RequestStoreFlags
 - ICEnroll3.RequestStoreFlags
 - ICEnroll3.get_RequestStoreFlags
 - ICEnroll3.put_RequestStoreFlags
 - ICEnroll2.RequestStoreFlags
 - ICEnroll2.get_RequestStoreFlags
 - ICEnroll2.put_RequestStoreFlags
 - ICEnroll.RequestStoreFlags
 - ICEnroll.get_RequestStoreFlags
 - ICEnroll.put_RequestStoreFlags
 - CEnroll.RequestStoreFlags
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICEnroll::get_RequestStoreFlags


## -description


<p class="CCE_Message">[This property is no longer available for use as of Windows Server 2008 and Windows Vista.]

The <b>RequestStoreFlags</b> property sets or retrieves the registry location used for the request store.

 The default value for this property  is CERT_SYSTEM_STORE_CURRENT_USER. This property was first defined in the <a href="https://msdn.microsoft.com/d5b746e0-91bd-45bd-9a67-ddc8868cee56">ICEnroll</a> interface.

This property is read/write.


## -parameters


## -remarks



The <b>RequestStoreFlags</b> property value is passed to the 
<a href="https://msdn.microsoft.com/4edccbfe-c0a8-442b-b6b7-51ef598e7c90">CertOpenStore</a> CryptoAPI function  by using its <i>dwFlags</i> parameter.

Typically, modification of the <b>RequestStoreFlags</b> property is  performed only in advanced applications.


The <b>RequestStoreFlags</b> property should be set before using the following methods:

<ul>
<li>
<a href="https://msdn.microsoft.com/5a428d83-c846-4f44-a682-58c3e025c353">acceptPKCS7</a>
</li>
<li>
<a href="https://msdn.microsoft.com/dae9f6b8-6690-47cc-9397-168c1ff54c55">acceptFilePKCS7</a>
</li>
<li>
<a href="https://msdn.microsoft.com/b8e841c1-f16e-4f3a-94f2-ef6708c88910">createPKCS10</a>
</li>
<li>
<a href="https://msdn.microsoft.com/074c7321-6117-4261-836a-a2055c9e029d">createFilePKCS10</a>
</li>
</ul>



#### Examples


```cpp
DWORD    dwFlags;
HRESULT  hr;

// pEnroll is previously instantiated ICEnroll interface pointer

// retrieve the flag value
hr = pEnroll->get_RequestStoreFlags( &dwFlags );
if ( FAILED ( hr ) )
    printf("Failed retrieving RequestStoreFlags - %x\n", hr );
else
    printf("RequestStoreFlags is %x\n", dwFlags );

// set the flag
hr = pEnroll->put_RequestStoreFlags
   ( CERT_SYSTEM_STORE_LOCAL_MACHINE );
if ( FAILED ( hr ) )
    printf("Failed updating RequestStoreFlags - %x\n", hr );
else
    printf("Updated RequestStoreFlags\n");
```



