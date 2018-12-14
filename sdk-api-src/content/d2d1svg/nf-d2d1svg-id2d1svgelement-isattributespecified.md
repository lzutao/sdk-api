---
UID: NF:d2d1svg.ID2D1SvgElement.IsAttributeSpecified
title: ID2D1SvgElement::IsAttributeSpecified
author: windows-sdk-content
description: Returns a boolean indicating if the attribute is explicitly set on the element.
old-location: direct2d\id2d1svgelement_isattributespecified.htm
tech.root: direct2d
ms.assetid: 94B91C4E-B2E5-4E23-B381-5920EA0F8F31
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID2D1SvgElement interface [Direct2D],IsAttributeSpecified method, ID2D1SvgElement.IsAttributeSpecified, ID2D1SvgElement::IsAttributeSpecified, IsAttributeSpecified, IsAttributeSpecified method [Direct2D], IsAttributeSpecified method [Direct2D],ID2D1SvgElement interface, d2d1svg/ID2D1SvgElement::IsAttributeSpecified, direct2d.id2d1svgelement_isattributespecified
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
 - ID2D1SvgElement.IsAttributeSpecified
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1SvgElement::IsAttributeSpecified


## -description


Returns a boolean indicating if the attribute is explicitly set on the element.


## -parameters




### -param name [in]

Type: <b>PCWSTR</b>

The name of the attribute.


### -param inherited [out, optional]

Type: <b>BOOL*</b>

Outputs whether the attribute is set to the inherit value.


## -returns



Type: <b>BOOL</b>

TReturns true if the attribute is explicitly set on the element or if it is present within an inline style. Returns FALSE if the attribute is not a valid
            attribute on this element.
          




## -see-also




<a href="https://msdn.microsoft.com/19099DC9-EA14-41C5-A9DF-5EBB12696C79">ID2D1SvgElement</a>
 

 
