---
UID: NN:ocidl.IPictureDisp
title: IPictureDisp
author: windows-sdk-content
description: Exposes the picture object's properties through Automation. It provides a subset of the functionality available through IPicture methods.
old-location: com\ipicturedisp.htm
tech.root: com
ms.assetid: 42efa5a3-66af-4432-a2fd-616261b1f407
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IPictureDisp, IPictureDisp interface [COM], IPictureDisp interface [COM],described, _ctrl_ipicturedisp, com.ipicturedisp, ocidl/IPictureDisp
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: ocidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: OCIdl.idl
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
 - COM
api_location:
 - OCIdl.h
api_name:
 - IPictureDisp
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IPictureDisp interface


## -description


Exposes the picture object's properties through Automation. It provides a subset of the functionality available through <a href="https://msdn.microsoft.com/42e3cd0e-2413-494a-8be8-2952089e02d2">IPicture</a> methods.


## -remarks



The following table describes the dispIDs for the various picture properties.

<table>
<tr>
<th>Constant</th>
<th>Value</th>
</tr>
<tr>
<td>DISPID_PICT_HANDLE
</td>
<td>0</td>
</tr>
<tr>
<td>DISPID_PICT_HPAL
</td>
<td>2</td>
</tr>
<tr>
<td>DISPID_PICT_TYPE
</td>
<td>3</td>
</tr>
<tr>
<td>DISPID_PICT_WIDTH
</td>
<td>4</td>
</tr>
<tr>
<td>DISPID_PICT_HEIGHT
</td>
<td>5</td>
</tr>
<tr>
<td>DISPID_PICT_RENDER
</td>
<td>6</td>
</tr>
</table>
 

Each property in the <b>IPictureDisp</b> interface includes a <b>get_PropertyName</b> method if the property supports read access and a <b>put_PropertyName</b> method if the property supports write access. Most of the properties support read access only with the exception of the hPal property.

<table>
<tr>
<th>Property</th>
<th>Type</th>
<th>Access</th>
<th>Description</th>
</tr>
<tr>
<td>Handle</td>
<td><b>OLE_HANDLE</b> (<b>int</b>)
</td>
<td>R</td>
<td>The Windows GDI handle of the picture
</td>
</tr>
<tr>
<td>hPal</td>
<td><b>OLE_HANDLE</b> (<b>int</b>)
</td>
<td>RW</td>
<td>The Windows handle of the palette used by the picture.
</td>
</tr>
<tr>
<td>Type</td>
<td><b>short</b></td>
<td>R</td>
<td>The type of picture (see <a href="https://msdn.microsoft.com/79f10687-f0eb-4b5e-a1a9-9186dbd0b51f">PICTYPE</a>).
</td>
</tr>
<tr>
<td>Width</td>
<td><b>OLE_XSIZE_HIMETRIC</b> (<b>long</b>)
</td>
<td>R</td>
<td>The width of the picture.
</td>
</tr>
<tr>
<td>Height</td>
<td><b>OLE_YSIZE_HIMETRIC</b> (<b>long</b>)
</td>
<td>R</td>
<td>The height of the picture.
</td>
</tr>
</table>
 

<h3><a id="OLE_Implementation"></a><a id="ole_implementation"></a><a id="OLE_IMPLEMENTATION"></a>OLE Implementation</h3>
Picture objects provide a language-neutral abstraction for bitmaps, icons, and metafiles. As with the standard font object, the system provides a standard implementation of the picture object. Its primary interfaces are <a href="https://msdn.microsoft.com/42e3cd0e-2413-494a-8be8-2952089e02d2">IPicture</a> and <b>IPictureDisp</b>. A picture object is created with <a href="https://msdn.microsoft.com/fb021348-07d4-4974-a71e-abb1b8d760c4">OleCreatePictureIndirect</a> and supports both the <b>IPicture</b> and the <b>IPictureDisp</b> interfaces.

The OLE-provided picture object implements the complete semantics of the <a href="https://msdn.microsoft.com/42e3cd0e-2413-494a-8be8-2952089e02d2">IPicture</a> and <b>IPictureDisp</b> interfaces.




## -see-also




<a href="https://msdn.microsoft.com/42e3cd0e-2413-494a-8be8-2952089e02d2">IPicture</a>
 

 
