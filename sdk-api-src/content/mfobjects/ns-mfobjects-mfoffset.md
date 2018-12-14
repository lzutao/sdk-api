---
UID: NS:mfobjects._MFOffset
title: MFOffset
author: windows-sdk-content
description: Specifies an offset as a fixed-point real number.
old-location: mf\mfoffset.htm
tech.root: medfound
ms.assetid: e93539fe-3e4a-4b34-8d6a-b3f300a70ffc
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MFOffset, MFOffset structure [Media Foundation], e93539fe-3e4a-4b34-8d6a-b3f300a70ffc, mf.mfoffset, mfobjects/MFOffset
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: mfobjects.h
req.include-header: Mfidl.h
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
 - mfobjects.h
api_name:
 - MFOffset
product: Windows
targetos: Windows
req.typenames: MFOffset
req.redist: 
---

# MFOffset structure


## -description


Specifies an offset as a fixed-point real number.
        


## -struct-fields




### -field fract

The fractional part of the number.
          


### -field value

The integer part of the number.
          


## -remarks



The value of the number is <b>value</b> + (<b>fract</b> / 65536.0f).


#### Examples

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>MFOffset MakeOffset(float v)
{
    MFOffset offset;
    offset.value = short(v);
    offset.fract = WORD(65536 * (v-offset.value));
    return offset;
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/39fdd724-13ca-48ab-8a55-93529d1da3b4">Media Foundation Structures</a>
 

 
