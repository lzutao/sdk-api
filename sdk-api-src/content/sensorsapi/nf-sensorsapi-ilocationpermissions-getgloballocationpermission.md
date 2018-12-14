---
UID: NF:sensorsapi.ILocationPermissions.GetGlobalLocationPermission
title: ILocationPermissions::GetGlobalLocationPermission
author: windows-sdk-content
description: Gets the status of the system setting that allows users to change location settings.
old-location: winsensors_com_ref\ilocationpermissions_getgloballocationpermission.htm
tech.root: SensorsAPI
ms.assetid: 8a2fbf9f-4b9b-4d2b-8ffc-c9491f7b8ed1
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetGlobalLocationPermission, GetGlobalLocationPermission method, GetGlobalLocationPermission method,ILocationPermissions interface, ILocationPermissions interface,GetGlobalLocationPermission method, ILocationPermissions.GetGlobalLocationPermission, ILocationPermissions::GetGlobalLocationPermission, sensorsapi/ILocationPermissions::GetGlobalLocationPermission, winsensors_com_ref.ilocationpermissions_getgloballocationpermission
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: sensorsapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Sensorsapi.lib
req.dll: Sensorsapi.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - sensorsapi.dll
api_name:
 - ILocationPermissions.GetGlobalLocationPermission
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ILocationPermissions::GetGlobalLocationPermission


## -description


Gets the status of the system setting that allows users to change location settings.


## -parameters




### -param pfEnabled [out]

<b>TRUE</b> if system settings allow users to enable or disable the location platform; otherwise, <b>FALSE</b>.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

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
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
NULL was passed in for pfEnabled.

</td>
</tr>
</table>
 




## -remarks



<div class="alert"><b>Note</b>  <b>GetGlobalLocationPermission</b> is available in Windows 8.</div>
<div> </div>
For more information on location settings in Windows 8 see <a href="https://msdn.microsoft.com/A1FC58B2-D455-4DF7-A4F7-EE0A7E8851DB">Location settings</a>.




## -see-also




<a href="https://msdn.microsoft.com/f4b46f4a-60be-4428-a4b5-6100ae3f1e1b">ILocationPermissions</a>
 

 
