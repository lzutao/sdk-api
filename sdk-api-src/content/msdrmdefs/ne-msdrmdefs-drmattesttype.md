---
UID: NE:msdrmdefs._DRMATTESTTYPE
title: DRMATTESTTYPE
author: windows-sdk-content
description: The DRMATTESTTYPE enumeration specifies what kind of signature to create for a data blob.
old-location: rm\drmattesttype.htm
tech.root: AdRms_Sdk
ms.assetid: adbf8718-e707-4ab9-a961-f8b4b4e1fe6a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DRMATTESTTYPE, DRMATTESTTYPE enumeration [Active Directory Rights Management Services SDK 1.0], DRMATTESTTYPE_FULLENVIRONMENT, DRMATTESTTYPE_HASHONLY, msdrmdefs/DRMATTESTTYPE, msdrmdefs/DRMATTESTTYPE_FULLENVIRONMENT, msdrmdefs/DRMATTESTTYPE_HASHONLY, rm.drmattesttype
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
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
 - DRMATTESTTYPE
product: Windows
targetos: Windows
req.typenames: DRMATTESTTYPE
req.redist: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# DRMATTESTTYPE enumeration


## -description


<p class="CCE_Message">[The AD RMS SDK leveraging functionality exposed by 

the client in Msdrm.dll is available for use in Windows Server 2008, Windows Vista, Windows Server 2008 R2, Windows 7, Windows Server 2012, and Windows 8. It may be altered or 

unavailable in subsequent versions. Instead, use <a href="https://msdn.microsoft.com/a7900f40-4c53-4760-8e5a-9c88149f86d0">Active Directory Rights Management Services SDK 2.1</a>, 

which leverages functionality exposed by the client in Msipc.dll.]

The <b>DRMATTESTTYPE</b> enumeration specifies what kind of signature to create for a data blob.


## -enum-fields




### -field DRMATTESTTYPE_FULLENVIRONMENT

Create a signature using full environment information.


### -field DRMATTESTTYPE_HASHONLY

Create a signature using only a hash of the environment.


## -see-also




<a href="https://msdn.microsoft.com/bc3a8ab3-9f89-442b-9910-85820b2b2653">AD RMS Enumerations</a>



<a href="https://msdn.microsoft.com/f0975845-d609-4f7a-a663-6481334c983d">DRMAttest</a>
 

 
