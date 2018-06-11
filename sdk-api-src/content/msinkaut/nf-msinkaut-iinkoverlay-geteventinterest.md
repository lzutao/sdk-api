---
UID: NF:msinkaut.IInkOverlay.GetEventInterest
title: IInkOverlay::GetEventInterest
author: windows-sdk-content
description: Retrieves the interest an object has in a particular event for the InkCollector class, InkOverlay class, or InkPicture class.
old-location: tablet\inkoverlay_geteventinterest.htm
old-project: tablet
ms.assetid: 709ba46e-fc39-4b91-b145-72381a1195a1
ms.author: windowssdkdev
ms.date: 06/06/2018
ms.keywords: 532a798e-b434-4730-8c20-7ec60255f170, GetEventInterest, GetEventInterest method [Tablet PC], GetEventInterest method [Tablet PC],IInkOverlay interface, IInkOverlay interface [Tablet PC],GetEventInterest method, IInkOverlay.GetEventInterest, IInkOverlay::GetEventInterest, msinkaut/IInkOverlay::GetEventInterest, tablet.inkoverlay_geteventinterest
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: msinkaut.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
tech.root: 
req.typenames: TabletPropertyMetricUnit
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - InkObj.dll
 - InkObj.dll.dll
api_name:
 - IInkOverlay.GetEventInterest
product: Windows
targetos: Windows
req.lib: InkObj.dll
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# IInkOverlay::GetEventInterest


## -description



Retrieves the interest an object has in a particular event for the <a href="https://msdn.microsoft.com/189f430e-9d00-4e29-bb8c-8ac195896793">InkCollector</a> class, <a href="https://msdn.microsoft.com/61191ab3-075e-458b-9e0f-4bc255687b3c">InkOverlay</a> class, or <a href="https://msdn.microsoft.com/e9fa6807-6e2a-44ec-9b8f-a560185e4367">InkPicture</a> class.




## -parameters




### -param EventId [in]

The event in which the ink collector is or is not interested.


### -param Listen [out, retval]

<b>VARIANT_TRUE</b> if interest in the specified event has been set; otherwise, <b>VARIANT_FALSE</b>.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
A parameter contained an invalid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid event interest.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INK_EXCEPTION</b></dt>
</dl>
</td>
<td width="60%">
An exception occurred during processing.

</td>
</tr>
</table>
 




## -see-also




<a href="tablet.iinkoverlay">IInkOverlay</a>



<a href="https://msdn.microsoft.com/db575790-345b-48da-b509-927eb2f47987">InkCollectorEventInterest Enumeration</a>



<a href="https://msdn.microsoft.com/61191ab3-075e-458b-9e0f-4bc255687b3c">InkOverlay Class</a>



<a href="https://msdn.microsoft.com/df25efbb-5229-4211-948f-3a213154a967">SetEventInterest Method</a>
 

 
