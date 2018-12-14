---
UID: NS:winnt._ENCLAVE_INIT_INFO_VBS
title: ENCLAVE_INIT_INFO_VBS
author: windows-sdk-content
description: Contains architecture-specific information to use to initialize an enclave when the enclave type is ENCLAVE_TYPE_VBS, which specifies a virtualization-based security (VBS) enclave.
old-location: base\enclave_init_info_vbs.htm
tech.root: memory
ms.assetid: 93DA44C6-6776-4682-84C2-347192669C77
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PENCLAVE_INIT_INFO_VBS, ENCLAVE_INIT_INFO_VBS, ENCLAVE_INIT_INFO_VBS structure, PENCLAVE_INIT_INFO_VBS, PENCLAVE_INIT_INFO_VBS structure pointer, base.enclave_init_info_vbs, winnt/ENCLAVE_INIT_INFO_VBS, winnt/PENCLAVE_INIT_INFO_VBS"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winnt.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1709 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
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
 - winnt.h
api_name:
 - ENCLAVE_INIT_INFO_VBS
product: Windows
targetos: Windows
req.typenames: ENCLAVE_INIT_INFO_VBS, *PENCLAVE_INIT_INFO_VBS
req.redist: 
---

# ENCLAVE_INIT_INFO_VBS structure


## -description


Contains architecture-specific information to use to initialize an enclave when the enclave type is <b>ENCLAVE_TYPE_VBS</b>, which specifies a virtualization-based security (VBS) enclave.


## -struct-fields




### -field Length

The total length of the <b>ENCLAVE_INIT_INFO_VBS</b> structure, in bytes.


### -field ThreadCount

Upon entry to the <a href="https://msdn.microsoft.com/6A711135-A522-40AE-965F-E1AF97D0076A">InitializeEnclave</a> function, specifies the number of threads to create in the enclave. Upon successful return from <b>InitializeEnclave</b>, contains the number of threads the function actually created.


## -see-also




<a href="https://msdn.microsoft.com/6A711135-A522-40AE-965F-E1AF97D0076A">InitializeEnclave</a>
 

 
