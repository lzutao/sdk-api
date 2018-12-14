---
UID: NS:msdrmdefs._DRM_ACTSERV_INFO
title: DRM_ACTSERV_INFO
author: windows-sdk-content
description: The DRM_ACTSERV_INFO structure stores information about the activation server.
old-location: rm\drm_actserv_info.htm
tech.root: AdRms_Sdk
ms.assetid: 2ea83a08-ab86-4635-8684-519808430ce9
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DRM_ACTSERV_INFO, DRM_ACTSERV_INFO structure [Active Directory Rights Management Services SDK 1.0], msdrmdefs/DRM_ACTSERV_INFO, rm.drm_actserv_info
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: msdrmdefs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - Msdrmdefs.h
api_name:
 - DRM_ACTSERV_INFO
product: Windows
targetos: Windows
req.typenames: DRM_ACTSERV_INFO
req.redist: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# DRM_ACTSERV_INFO structure


## -description


<p class="CCE_Message">[The AD RMS SDK leveraging functionality exposed by 

the client in Msdrm.dll is available for use in Windows Server 2008, Windows Vista, Windows Server 2008 R2, Windows 7, Windows Server 2012, and Windows 8. It may be altered or 

unavailable in subsequent versions. Instead, use <a href="https://msdn.microsoft.com/a7900f40-4c53-4760-8e5a-9c88149f86d0">Active Directory Rights Management Services SDK 2.1</a>, 

which leverages functionality exposed by the client in Msipc.dll.]

The <b>DRM_ACTSERV_INFO</b> structure stores information about the activation server.


## -struct-fields




### -field uVersion

Version of this structure, for backward compatibility. When using C, this value should be initialized to <b>DRMACTSERVINFOVERSION</b>. In C++ this is done automatically.


### -field wszPubKey

This member is reserved and must be set to <b>NULL</b>.


### -field wszURL

URL for a service that performs activation. Use <a href="https://msdn.microsoft.com/f7cbc3ba-009f-4a35-999e-139d41961fd9">DRMGetServiceLocation</a> to find a service location if none is known, or pass in <b>NULL</b> to use Passport service discovery. The URL should have the form <b>http://</b><i>CompanyName</i><b>/_wmcs/certification</b>, for example, http://blueyonderairlines/_wmcs/certification. The parameter defaults to <b>NULL</b> in C++.


### -field _DRM_ACTSERV_INFO

TBD 




## -remarks



This structure has a C++ default constructor that takes no parameters and sets members to the default values described above.




## -see-also




<a href="https://msdn.microsoft.com/06a0c6d2-108d-4c72-9ae6-8959304602c5">AD RMS Structures</a>



<a href="https://msdn.microsoft.com/d3f4ac2c-95d9-4273-a679-81670dd62d28">DRMActivate</a>



<a href="https://msdn.microsoft.com/f6c7bc7f-e9e8-4fc4-b30f-31bc0f5f46aa">DRMIsActivated</a>
 

 
