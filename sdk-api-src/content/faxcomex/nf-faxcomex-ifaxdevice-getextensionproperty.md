---
UID: NF:faxcomex.IFaxDevice.GetExtensionProperty
title: IFaxDevice::GetExtensionProperty
author: windows-sdk-content
description: The IFaxDevice::get_GetExtensionProperty method retrieves an extension configuration property stored at the device level.
old-location: fax\_mfax_faxdevice_cpp_mfax_faxdevice_getextensionproperty_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_94e1.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetExtensionProperty, GetExtensionProperty method [Fax Service], GetExtensionProperty method [Fax Service],IFaxDevice interface, IFaxDevice interface [Fax Service],GetExtensionProperty method, IFaxDevice.GetExtensionProperty, IFaxDevice::GetExtensionProperty, _mfax_faxdevice.getextensionproperty, fax._mfax_faxdevice_cpp_mfax_faxdevice_getextensionproperty_cpp, fax._mfax_faxdevice_getextensionproperty, faxcomex/IFaxDevice::GetExtensionProperty
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcomex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fxscomex.dll
api_name:
 - IFaxDevice.GetExtensionProperty
 - IFaxDevice.GetExtensionProperty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxDevice::GetExtensionProperty


## -description


The <b>IFaxDevice::get_GetExtensionProperty</b> method retrieves an extension configuration property stored at the device level.


## -parameters




### -param bstrGUID [in]

Type: <b>BSTR</b>

Specifies a string GUID that uniquely identifies the data to be retrieved.


### -param pvProperty

TBD




#### - vProperty [out, retval]

Type: <b>VARIANT*</b>

<b>VARIANT</b> that specifies the data.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



<div class="alert"><b>Note</b>  The returned data is a blob of bytes represented as a variant safe array of unsigned chars (VT_UI1 | VT_ARRAY). The data is relevant only to the specific extension that uses it. For more information see <a href="https://msdn.microsoft.com/en-us/library/ms684522(v=VS.85).aspx">About the Fax Extension Configuration API</a>.</div>
<div> </div>
To use this method, a user must have the <a href="https://msdn.microsoft.com/en-us/library/ms689205(v=VS.85).aspx">farQUERY_CONFIG</a> access right.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms686192(v=VS.85).aspx">FaxDevice</a>



<a href="https://msdn.microsoft.com/en-us/library/ms686193(v=VS.85).aspx">IFaxDevice</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693437(v=VS.85).aspx">Visual Basic Example</a>
 

 
