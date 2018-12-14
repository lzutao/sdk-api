---
UID: NS:iads.__MIDL___MIDL_itf_ads_0000_0000_0008
title: ADS_BACKLINK
author: windows-sdk-content
description: The ADS_BACKLINK structure is an ADSI representation of the Back Link attribute syntax.
old-location: adsi\ads_backlink.htm
tech.root: adsi
ms.assetid: 1352d304-b984-43ab-8c47-5108f35ae193
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PADS_BACKLINK, ADS_BACKLINK, ADS_BACKLINK structure [ADSI], PADS_BACKLINK, PADS_BACKLINK structure pointer [ADSI], _ds_ads_backlink, adsi.ads__backlink, adsi.ads_backlink, iads/ADS_BACKLINK, iads/PADS_BACKLINK"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: iads.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
 - Iads.h
api_name:
 - ADS_BACKLINK
product: Windows
targetos: Windows
req.typenames: ADS_BACKLINK, *PADS_BACKLINK
req.redist: 
---

# ADS_BACKLINK structure


## -description


The <b>ADS_BACKLINK</b> structure is an ADSI representation of the <b>Back Link</b> attribute syntax.


## -struct-fields




### -field RemoteID

Identifier of the remote server that requires an external reference to the object specified by <b>ObjectName</b>. See below.


### -field ObjectName

The null-terminated Unicode string that specifies the name of an object to which the <b>Back Link</b> attribute is attached.


## -remarks



A <b>Back Link</b> attribute contains one or more servers that hold an external reference to the attached object.




## -see-also




<a href="https://msdn.microsoft.com/3ee0e469-9932-4135-8798-27d318011786">ADSI Structures</a>
 

 
