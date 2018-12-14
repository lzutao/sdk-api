---
UID: NN:d2d1svg.ID2D1SvgAttribute
title: ID2D1SvgAttribute
author: windows-sdk-content
description: Interface describing an SVG attribute.
old-location: direct2d\id2d1svgattribute.htm
tech.root: direct2d
ms.assetid: 7B11D05C-6CD5-4609-B76A-719B92437314
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ID2D1SvgAttribute, ID2D1SvgAttribute interface [Direct2D], ID2D1SvgAttribute interface [Direct2D],described, d2d1svg/ID2D1SvgAttribute, direct2d.id2d1svgattribute
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
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
 - ID2D1SvgAttribute
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1SvgAttribute interface


## -description


Interface describing an SVG attribute.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ID2D1SvgAttribute</b> interface inherits from <a href="https://msdn.microsoft.com/8f19e74a-f010-4082-a4da-d1dc3cfe3192">ID2D1Resource</a>. <b>ID2D1SvgAttribute</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ID2D1SvgAttribute</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/85A16E88-5010-403F-B6B9-EBA6A4321463">Clone</a>
</td>
<td align="left" width="63%">
Creates a clone of this attribute value. On creation, the cloned attribute is not set on any element.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/F02A13BF-955A-4D74-BC12-F1E6DCFFCCE9">GetElement</a>
</td>
<td align="left" width="63%">
Returns the element on which this attribute is set. Returns null if the attribute is not set on any element.

</td>
</tr>
</table> 
