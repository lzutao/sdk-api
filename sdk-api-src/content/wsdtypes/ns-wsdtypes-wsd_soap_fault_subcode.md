---
UID: NS:wsdtypes._WSD_SOAP_FAULT_SUBCODE
title: WSD_SOAP_FAULT_SUBCODE
author: windows-sdk-content
description: Represents a generated SOAP fault subcode.
old-location: ncd\wsd_soap_fault_subcode_struct.htm
tech.root: wsdapi
ms.assetid: cd8f35e4-7b22-4af0-b6a4-78f43ed8b060
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WSD_SOAP_FAULT_SUBCODE, WSD_SOAP_FAULT_SUBCODE structure, ncd.wsd_soap_fault_subcode_struct, wsdtypes/WSD_SOAP_FAULT_SUBCODE
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: wsdtypes.h
req.include-header: Wsdapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - WsdTypes.h
api_name:
 - WSD_SOAP_FAULT_SUBCODE
product: Windows
targetos: Windows
req.typenames: WSD_SOAP_FAULT_SUBCODE
req.redist: 
---

# WSD_SOAP_FAULT_SUBCODE structure


## -description


Represents a generated SOAP fault subcode.  Subcodes can be nested.


## -struct-fields




### -field Value

A <a href="https://msdn.microsoft.com/9dce71d2-700c-4f86-9308-dee6a69010bb">WSDXML_NAME</a> structure that contains the  qualified name of the SOAP fault subcode.


### -field Subcode

A <b>WSD_SOAP_FAULT_SUBCODE</b> structure that contains a fault subcode.


## -see-also




<a href="https://msdn.microsoft.com/b71f4bcc-d125-4091-a491-1a5a2aea2310">WSD_SOAP_FAULT_CODE</a>
 

 
