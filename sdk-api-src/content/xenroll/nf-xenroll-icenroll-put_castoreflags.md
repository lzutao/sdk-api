---
UID: NF:xenroll.ICEnroll.put_CAStoreFlags
title: ICEnroll::put_CAStoreFlags
author: windows-sdk-content
description: Sets or retrieves a flag that controls the certification authority (CA) store when the store is opened.
old-location: security\icenroll4_castoreflags.htm
tech.root: seccrypto
ms.assetid: cde75e0f-5074-44f7-a101-f503913a58f4
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CAStoreFlags property [Security], CAStoreFlags property [Security],CEnroll object, CAStoreFlags property [Security],ICEnroll interface, CAStoreFlags property [Security],ICEnroll2 interface, CAStoreFlags property [Security],ICEnroll3 interface, CAStoreFlags property [Security],ICEnroll4 interface, CEnroll object [Security],CAStoreFlags property, ICEnroll interface [Security],CAStoreFlags property, ICEnroll.CAStoreFlags, ICEnroll.put_CAStoreFlags, ICEnroll2 interface [Security],CAStoreFlags property, ICEnroll2.CAStoreFlags, ICEnroll2::get_CAStoreFlags, ICEnroll2::put_CAStoreFlags, ICEnroll3 interface [Security],CAStoreFlags property, ICEnroll3.CAStoreFlags, ICEnroll3::get_CAStoreFlags, ICEnroll3::put_CAStoreFlags, ICEnroll4 interface [Security],CAStoreFlags property, ICEnroll4.CAStoreFlags, ICEnroll4::CAStoreFlags, ICEnroll4::get_CAStoreFlags, ICEnroll4::put_CAStoreFlags, ICEnroll::get_CAStoreFlags, ICEnroll::put_CAStoreFlags, put_CAStoreFlags, security.icenroll4_castoreflags, xenroll/ICEnroll2::CAStoreFlags, xenroll/ICEnroll2::get_CAStoreFlags, xenroll/ICEnroll2::put_CAStoreFlags, xenroll/ICEnroll3::CAStoreFlags, xenroll/ICEnroll3::get_CAStoreFlags, xenroll/ICEnroll3::put_CAStoreFlags, xenroll/ICEnroll4::CAStoreFlags, xenroll/ICEnroll4::get_CAStoreFlags, xenroll/ICEnroll4::put_CAStoreFlags, xenroll/ICEnroll::CAStoreFlags, xenroll/ICEnroll::get_CAStoreFlags, xenroll/ICEnroll::put_CAStoreFlags
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
 - ICEnroll4.CAStoreFlags
 - ICEnroll4.get_CAStoreFlags
 - ICEnroll4.put_CAStoreFlags
 - ICEnroll3.CAStoreFlags
 - ICEnroll3.get_CAStoreFlags
 - ICEnroll3.put_CAStoreFlags
 - ICEnroll2.CAStoreFlags
 - ICEnroll2.get_CAStoreFlags
 - ICEnroll2.put_CAStoreFlags
 - ICEnroll.CAStoreFlags
 - ICEnroll.get_CAStoreFlags
 - ICEnroll.put_CAStoreFlags
 - CEnroll.CAStoreFlags
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICEnroll::put_CAStoreFlags


## -description


<p class="CCE_Message">[This property is no longer available for use as of Windows Server 2008 and Windows Vista.]

The <b>CAStoreFlags</b> property sets or retrieves a flag that controls the <a href="https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb">certification authority</a> (CA) store when the store is opened. This flag is  passed to the <i>dwFlags</i> parameter of the <a href="https://msdn.microsoft.com/4edccbfe-c0a8-442b-b6b7-51ef598e7c90">CertOpenStore</a> function when the CA store is opened.

The default value for this property is CERT_SYSTEM_STORE_CURRENT_USER.  This property was first defined in the <a href="https://msdn.microsoft.com/d5b746e0-91bd-45bd-9a67-ddc8868cee56">ICEnroll</a> interface.

This property is read/write.


## -parameters


## -remarks




The <b>CAStoreFlags</b> property affects the behavior of the following methods:

<ul>
<li>
<a href="https://msdn.microsoft.com/5a428d83-c846-4f44-a682-58c3e025c353">acceptPKCS7</a>
</li>
<li>
<a href="https://msdn.microsoft.com/dae9f6b8-6690-47cc-9397-168c1ff54c55">acceptFilePKCS7</a>
</li>
</ul>



#### Examples


```cpp
DWORD    dwFlags;
HRESULT  hr;

// pEnroll is previously instantiated ICEnroll interface pointer

// retrieve the flag value
hr = pEnroll->get_CAStoreFlags( &dwFlags );
if ( FAILED ( hr ) )
    printf("Failed retrieving CAStoreFlags - %x\n", hr );
else
    printf("CAStoreFlags is %x\n", dwFlags );

// set the flag
hr = pEnroll->put_CAStoreFlags( CERT_SYSTEM_STORE_LOCAL_MACHINE );
if ( FAILED ( hr ) )
    printf("Failed updating CAStoreFlags - %x\n", hr );
else
    printf("Updated CAStoreFlags\n");
```



