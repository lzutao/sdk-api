---
UID: NF:msinkaut.IInkRenderer.MeasureStroke
title: IInkRenderer::MeasureStroke
author: windows-sdk-content
description: Calculates the rectangle on the device context that would contain a stroke if it were drawn with the InkRenderer object using the DrawStroke method.
old-location: tablet\inkrenderer_measurestroke.htm
tech.root: tablet
ms.assetid: bdaee1c8-ff03-470f-b508-3db5391b3cf7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IInkRenderer interface [Tablet PC],MeasureStroke method, IInkRenderer.MeasureStroke, IInkRenderer::MeasureStroke, MeasureStroke, MeasureStroke method [Tablet PC], MeasureStroke method [Tablet PC],IInkRenderer interface, bdaee1c8-ff03-470f-b508-3db5391b3cf7, msinkaut/IInkRenderer::MeasureStroke, tablet.inkrenderer_measurestroke
ms.prod: windows-hardware
ms.technology: windows-devices
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
req.lib: InkObj.dll
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - InkObj.dll
 - InkObj.dll.dll
api_name:
 - IInkRenderer.MeasureStroke
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IInkRenderer::MeasureStroke


## -description



Calculates the rectangle on the device context that would contain a stroke if it were drawn with the <a href="https://msdn.microsoft.com/66ec7cab-bfc2-4934-93a4-0ab9cb8c96e7">InkRenderer</a> object using the <a href="https://msdn.microsoft.com/3d8b7892-a120-452a-b83c-474df9be5f52">DrawStroke</a> method.




## -parameters




### -param Stroke [in]

The stroke to measure.


### -param DrawingAttributes [in, optional]

Optional. The <a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttributes</a> to use when calculating the rectangle, which override the drawing attributes on the stroke. The default value is <b>NULL</b>, which means the stroke is measured by using its own drawing attributes.


### -param Rectangle [out, retval]

When this method returns, contains a pointer to the rectangle on the device context that would contain the stroke if the stroke were drawn with the <a href="https://msdn.microsoft.com/3d8b7892-a120-452a-b83c-474df9be5f52">DrawStroke</a> method of the <a href="https://msdn.microsoft.com/66ec7cab-bfc2-4934-93a4-0ab9cb8c96e7">InkRenderer</a> object. The stroke must contain x- and y-coordinates to calculate the rectangle. Otherwise, the method returns an empty rectangle.


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
<dt><b>REGDB_E_CLASSNOTREG</b></dt>
</dl>
</td>
<td width="60%">
The <a href="https://msdn.microsoft.com/78e6c29c-0f43-46a5-9d30-948de5f369c8">InkRectangle</a> object is not registered on the system.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INK_INCOMPATIBLE_OBJECT</b></dt>
</dl>
</td>
<td width="60%">

<a href="https://msdn.microsoft.com/b18464ba-feb6-4bb5-9fcf-82feff9bcce4">IInkStrokeDisp</a> does not point to a compatible <a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp</a> object, or <i>drawingAttributes</i> is an invalid input parameter.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INK_EXCEPTION</b></dt>
</dl>
</td>
<td width="60%">
An exception occurred inside the method.

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
Invalid display handle.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
Unexpected parameter or property type.

</td>
</tr>
</table>
 




## -remarks



This is accurate only if you pass the same arguments to both <b>MeasureStroke</b> and <a href="https://msdn.microsoft.com/3d8b7892-a120-452a-b83c-474df9be5f52">DrawStroke</a>.

Since the bounding box is affected by the pen width, this width is scaled appropriately for the <a href="https://msdn.microsoft.com/66ec7cab-bfc2-4934-93a4-0ab9cb8c96e7">InkRenderer</a>'s view transform. To do this, the pen width is multiplied by the square root of the determinant of the view transform. The height and width of the bounding box are expanded by half this amount in each direction, and the right and bottom sides are incremented by one.

For example, consider that the pen width is originally 53, the square root of the determinant of the view transform is 50, and the bounding box is (0, 0, 1000, 1000). The pen width adjustment to the bounding box in each direction is calculated as (53 * 50) / 2, and the right and bottom sides are incremented by one. This results in a rendered bounding box of (-1325, -1325, 2326, 2326).




## -see-also




<a href="https://msdn.microsoft.com/18f67080-ed56-43af-b0d6-8af35c2e871b">Draw Method [InkRenderer Class]</a>



<a href="https://msdn.microsoft.com/3d8b7892-a120-452a-b83c-474df9be5f52">DrawStroke Method</a>



<a href="https://msdn.microsoft.com/en-us/library/Mt846805(v=VS.85).aspx">IInkRenderer</a>



<a href="https://msdn.microsoft.com/b18464ba-feb6-4bb5-9fcf-82feff9bcce4">IInkStrokeDisp Interface</a>



<a href="https://msdn.microsoft.com/66ec7cab-bfc2-4934-93a4-0ab9cb8c96e7">InkRenderer Class</a>



<a href="https://msdn.microsoft.com/1ef9ef91-ae96-454f-9ef8-570e64852395">Measure Method</a>
 

 
