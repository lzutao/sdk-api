---
UID: NF:msinkaut.IInkDrawingAttributes.put_Width
title: IInkDrawingAttributes::put_Width
author: windows-sdk-content
description: Gets or sets the y-axis dimension, or width, of the pen tip when drawing ink.
old-location: tablet\inkdrawingattributes_width.htm
old-project: tablet
ms.assetid: 6069f9d3-061a-48ba-8161-86d6152d68f0
ms.author: windowssdkdev
ms.date: 06/06/2018
ms.keywords: 6069f9d3-061a-48ba-8161-86d6152d68f0, IInkDrawingAttributes interface [Tablet PC],Width property, IInkDrawingAttributes.Width, IInkDrawingAttributes.put_Width, IInkDrawingAttributes::Width, IInkDrawingAttributes::get_Width, IInkDrawingAttributes::put_Width, InkDrawingAttributes.get_Width, InkDrawingAttributes.put_Width, Width property [Tablet PC], Width property [Tablet PC],IInkDrawingAttributes interface, get_Width, msinkaut/IInkDrawingAttributes::Width, msinkaut/IInkDrawingAttributes::get_Width, msinkaut/IInkDrawingAttributes::put_Width, put_Width, tablet.inkdrawingattributes_width
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
 - IInkDrawingAttributes.Width
 - IInkDrawingAttributes.get_Width
 - IInkDrawingAttributes.put_Width
 - InkDrawingAttributes.get_Width
 - InkDrawingAttributes.put_Width
product: Windows
targetos: Windows
req.lib: InkObj.dll
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# IInkDrawingAttributes::put_Width


## -description



Gets or sets the y-axis dimension, or width, of the pen tip when drawing ink.



This property is read/write.


## -parameters


## -remarks



If the tablet reports pen pressure (if the <a href="https://msdn.microsoft.com/adf5beec-75df-46a3-91e4-33595340aca2">IgnorePressure</a> property is false), the actual width of the ink varies depending on the amount of pressure applied to the drawing surface. When maximum pressure is applied, the width is 150% of the value of the <code>Width</code> property. When minimum pressure is applied, the width is 50% of the value of the <code>Width</code> property. By default, this property is set to true, so that pressure from the pen is reported. To specify that pressure should not be reported (that the width of ink does not change), set the <b>IgnorePressure</b> property to true.

Precision is limited to one one-thousandth of a HIMETRIC unit (three digits to the right of the decimal point). For example, if you specify a value of 2.0006, the most precise measurement is 2.001.




## -see-also




<a href="https://msdn.microsoft.com/2dc9eb94-649f-42f6-8180-abf570bdc757">Height Property [InkDrawingAttributes Class]</a>



<a href="tablet.iinkdrawingattributes">IInkDrawingAttributes</a>



<a href="https://msdn.microsoft.com/adf5beec-75df-46a3-91e4-33595340aca2">IgnorePressure Property</a>



<a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttributes Class</a>



<a href="https://msdn.microsoft.com/13e3c2dc-99a4-4643-b8b2-48586b0eb2f0">PenTip Property</a>
 

 
