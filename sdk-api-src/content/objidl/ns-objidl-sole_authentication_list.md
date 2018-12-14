---
UID: NS:objidl.tagSOLE_AUTHENTICATION_LIST
title: SOLE_AUTHENTICATION_LIST
author: windows-sdk-content
description: Indicates the default authentication information to use with each authentication service.
old-location: com\sole_authentication_list.htm
tech.root: com
ms.assetid: 21f7aef3-b6be-41cc-a6ed-16d3778e3cee
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSOLE_AUTHENTICATION_LIST, PSOLE_AUTHENTICATION_LIST, PSOLE_AUTHENTICATION_LIST structure pointer [COM], SOLE_AUTHENTICATION_LIST, SOLE_AUTHENTICATION_LIST structure [COM], _com_SOLE_AUTHENTICATION_LIST, com.sole_authentication_list, objidlbase/PSOLE_AUTHENTICATION_LIST, objidlbase/SOLE_AUTHENTICATION_LIST, tagSOLE_AUTHENTICATION_LIST"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: objidl.h
req.include-header: Objidl.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - objidlbase.h
api_name:
 - SOLE_AUTHENTICATION_LIST
product: Windows
targetos: Windows
req.typenames: SOLE_AUTHENTICATION_LIST, *PSOLE_AUTHENTICATION_LIST
req.redist: 
---

# SOLE_AUTHENTICATION_LIST structure


## -description


Indicates the default authentication information to use with each authentication service. When DCOM negotiates the default authentication service for a proxy, it picks the default authentication information from this list.



## -struct-fields




### -field cAuthInfo

The count of pointers in the array pointed to by <b>aAuthInfo</b>. 


### -field aAuthInfo

An array of <a href="https://msdn.microsoft.com/23beb1b1-e4b7-4282-9868-5caf40a69a61">SOLE_AUTHENTICATION_INFO</a> structures. Each of these structures contains an identifier for an authentication service, an identifier for the authorization service, and a pointer to authentication information to use with the specified authentication service.



## -see-also




<a href="https://msdn.microsoft.com/e0933741-6b75-4ce1-aa63-6240e4a7130f">CoInitializeSecurity</a>
 

 
