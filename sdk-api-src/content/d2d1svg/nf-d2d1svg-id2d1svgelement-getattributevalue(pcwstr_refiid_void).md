---
UID: NF:d2d1svg.ID2D1SvgElement.GetAttributeValue(PCWSTR,REFIID,void)
title: ID2D1SvgElement::GetAttributeValue(PCWSTR,REFIID,void)
author: windows-sdk-content
description: Gets an attribute of this element as an interface type.
old-location: direct2d\id2d1svgelement_getattributevalue_3.htm
tech.root: direct2d
ms.assetid: 5EDFBEB6-E28E-44BD-AE4C-1FCCD9D11EAB
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAttributeValue, GetAttributeValue method [Direct2D], GetAttributeValue method [Direct2D],ID2D1SvgElement interface, ID2D1SvgElement interface [Direct2D],GetAttributeValue method, ID2D1SvgElement.GetAttributeValue, ID2D1SvgElement.GetAttributeValue(PCWSTR,REFIID,void), ID2D1SvgElement::GetAttributeValue, ID2D1SvgElement::GetAttributeValue(PCWSTR,REFIID,void), d2d1svg/ID2D1SvgElement::GetAttributeValue, direct2d.id2d1svgelement_getattributevalue_3
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d2d1svg.h
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
req.dll: Direct2d.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - direct2d.dll
api_name:
 - ID2D1SvgElement.GetAttributeValue
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1SvgElement::GetAttributeValue(PCWSTR,REFIID,void)


## -description


Gets an attribute of this element as an interface type. 


## -parameters




### -param name [in]

Type: <b>PCWSTR</b>

The name of the attribute.


### -param riid [in]

Type: <b>REFIID</b>

The interface ID of the attribute value.


### -param value

Type: <b>void**</b>

The value of the attribute.


## -returns



Type: <b><a href="455d07e9-52c3-4efb-a9dc-2955cbfd38cc">HRESULT</a></b>

This method returns an HRESULT success or error code. Returns an error if the
     attribute is not specified. Returns an error if the attribute name is not valid
     on this element. Returns an error if the attribute cannot be expressed as the
     specified interface type.




## -see-also




<a href="https://msdn.microsoft.com/19099DC9-EA14-41C5-A9DF-5EBB12696C79">ID2D1SvgElement</a>
 

 
