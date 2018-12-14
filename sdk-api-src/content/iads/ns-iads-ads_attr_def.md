---
UID: NS:iads._ads_attr_def
title: ADS_ATTR_DEF
author: windows-sdk-content
description: The ADS_ATTR_DEF structure is used only as a part of IDirectorySchemaMgmt, which is an obsolete interface.
old-location: adsi\ads_attr_def.htm
tech.root: adsi
ms.assetid: 01cada92-e69a-40d4-a253-ad88c663fa92
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PADS_ATTR_DEF, ADS_ATTR_DEF, ADS_ATTR_DEF structure [ADSI], PADS_ATTR_DEF, PADS_ATTR_DEF structure pointer [ADSI], _ds_ads_attr_def, adsi.ads__attr__def, adsi.ads_attr_def, iads/ADS_ATTR_DEF, iads/PADS_ATTR_DEF"
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
 - ADS_ATTR_DEF
product: Windows
targetos: Windows
req.typenames: ADS_ATTR_DEF, *PADS_ATTR_DEF
req.redist: 
---

# ADS_ATTR_DEF structure


## -description


The <b>ADS_ATTR_DEF</b> structure is used only as a part of <b>IDirectorySchemaMgmt</b>, which is an obsolete interface.  The following information is provided for legacy purposes only.
   

The <b>ADS_ATTR_DEF</b> structure describes schema data for an attribute. It is used to manage attribute definitions in the schema.


## -struct-fields




### -field pszAttrName

The null-terminated Unicode string that contains the name of the attribute.


### -field dwADsType

Data type of the attribute as defined by  <a href="https://msdn.microsoft.com/e601bae5-80bf-43f5-846f-11327889419a">ADSTYPEENUM</a>.


### -field dwMinRange

Minimum legal range for this attribute.


### -field dwMaxRange

Maximum legal range for this attribute.


### -field fMultiValued

Whether or not this attribute takes more than one value.


## -remarks



In ADSI, attributes and properties are used interchangeably.




## -see-also




<a href="https://msdn.microsoft.com/3ee0e469-9932-4135-8798-27d318011786">ADSI Structures</a>



<a href="https://msdn.microsoft.com/e601bae5-80bf-43f5-846f-11327889419a">ADSTYPEENUM</a>
 

 
