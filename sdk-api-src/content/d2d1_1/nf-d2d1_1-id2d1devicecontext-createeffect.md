---
UID: NF:d2d1_1.ID2D1DeviceContext.CreateEffect
title: ID2D1DeviceContext::CreateEffect
author: windows-sdk-content
description: Creates an effect for the specified class ID.
old-location: direct2d\id2d1devicecontext_createeffect.htm
tech.root: direct2d
ms.assetid: dfe587f9-e92f-4367-a503-edd446a91cb8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CreateEffect, CreateEffect method [Direct2D], CreateEffect method [Direct2D],ID2D1DeviceContext interface, ID2D1DeviceContext interface [Direct2D],CreateEffect method, ID2D1DeviceContext.CreateEffect, ID2D1DeviceContext::CreateEffect, d2d1_1/ID2D1DeviceContext::CreateEffect, direct2d.id2d1devicecontext_createeffect
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d2d1_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
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
req.dll: D2d1.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D2d1.dll
api_name:
 - ID2D1DeviceContext.CreateEffect
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID2D1DeviceContext::CreateEffect


## -description


Creates an effect for the specified class ID. 


## -parameters




### -param effectId

Type: <b>REFCLSID</b>

The class ID of the effect to create. See <a href="https://msdn.microsoft.com/A76F6AB8-16E9-45C9-A768-5E4AA072D534">Built-in Effects</a> for a list of effect IDs.


### -param effect [out]

Type: <b><a href="https://msdn.microsoft.com/e90d1830-c356-48f1-ac7b-1d94c8c26569">ID2D1Effect</a>**</b>

When this method returns, contains the address of a pointer to a new effect.


## -returns



Type: <b>HRESULT</b>

The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.
            

<table>
<tr>
<th>HRESULT</th>
<th>Description</th>
</tr>
<tr>
<td>S_OK</td>
<td>No error occurred.</td>
</tr>
<tr>
<td>E_OUTOFMEMORY</td>
<td>Direct2D could not allocate sufficient memory to complete the call.
                </td>
</tr>
<tr>
<td>E_INVALIDARG</td>
<td>An invalid value was passed to the method.</td>
</tr>
<tr>
<td>D3DERR_OUTOFVIDEOMEMORY</td>
<td>Direct3D does not have enough display memory to perform the operation.
                </td>
</tr>
<tr>
<td>D2DERR_EFFECT_IS_NOT_REGISTERED</td>
<td>The specified effect is not registered by the system.</td>
</tr>
<tr>
<td>D2DERR_INSUFFICIENT_DEVICE_CAPABILITIES </td>
<td>The effect requires capabilities not supported by the D2D device.</td>
</tr>
</table>
 




## -remarks



If the  created effect is a custom effect that is implemented in a DLL, this doesn't increment the reference count for that DLL. 
        If the application deletes an effect while that effect is loaded, the resulting behavior is unpredictable.
      




## -see-also




<a href="https://msdn.microsoft.com/1446BDA9-AD4C-472C-8F1D-82ABC1880E13">Effects</a>



<a href="https://msdn.microsoft.com/a54dd628-c2a2-4b04-9ced-7749a395f187">ID2D1DeviceContext</a>



<a href="https://msdn.microsoft.com/e90d1830-c356-48f1-ac7b-1d94c8c26569">ID2D1Effect</a>



<a href="https://msdn.microsoft.com/9988aad6-0487-4f48-a05c-1dfb944f6ce7">ID2D1Factory1::RegisterEffect</a>
 

 
