---
UID: NF:locationapi.ILatLongReport.GetAltitude
title: ILatLongReport::GetAltitude
author: windows-sdk-content
description: Retrieves the altitude, in meters. Altitude is relative to the reference ellipsoid.
old-location: winlocation_com_ref\ilatlongreport_getaltitude.htm
tech.root: locationapi
ms.assetid: 7ab8e3fb-03da-4529-aaf0-3a178474e4a5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetAltitude, GetAltitude method [WinLocation], GetAltitude method [WinLocation],ILatLongReport interface, ILatLongReport interface [WinLocation],GetAltitude method, ILatLongReport.GetAltitude, ILatLongReport::GetAltitude, WinLocation_COM_Ref.ilatlongreport_getaltitude, locationapi/ILatLongReport::GetAltitude
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: locationapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only],Windows 7
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
req.lib: 
req.dll: LocationAPI.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - LocationAPI.dll
api_name:
 - ILatLongReport.GetAltitude
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ILatLongReport::GetAltitude


## -description


<p class="CCE_Message">[The Win32 Location API is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions. Instead, use the <a href="https://msdn.microsoft.com/fd40bf4a-c59a-43a4-ab01-c671a8a41731">Windows.Devices.Geolocation</a>API.
]

Retrieves the altitude, in meters. Altitude is relative to the reference ellipsoid.


## -parameters




### -param pAltitude [out]

Address of a <b>DOUBLE</b> that receives the altitude, in meters. May be <b>NULL</b>.


## -returns



Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>S_OK</dt>
</dl>
</td>
<td width="60%">
The method returned successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>HRESULT_FROM_WIN32(ERROR_NO_DATA)</dt>
</dl>
</td>
<td width="60%">
The location report does not include data for the requested field. This result is returned when the location sensor does not support altitude.

</td>
</tr>
</table>
 




## -remarks



The <b>GetAltitude</b> method retrieves the altitude relative to the reference ellipsoid that is defined by the latest revision of the World Geodetic System (WGS 84), rather than the altitude relative to sea level.


#### Examples

The following code example demonstrates how to call <b>GetAltitude</b>. Altitude is an optional field in latitude/longitude reports, so <b>GetAltitude</b> may not always return data.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>DOUBLE altitude = 0;
// Print the Altitude
if (SUCCEEDED(spLatLongReport-&gt;GetAltitude(&amp;altitude)))
{
    wprintf(L"Altitude: %f\n", altitude);
}
else
{
    // Altitude is optional and may not be available
    wprintf(L"Altitude: Not available.\n");
}
</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/b489959e-74c7-46df-b63f-7d37e3a244d5">ILatLongReport</a>
 

 
