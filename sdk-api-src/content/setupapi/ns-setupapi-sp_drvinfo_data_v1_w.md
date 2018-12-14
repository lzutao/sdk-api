---
UID: NS:setupapi._SP_DRVINFO_DATA_V1_W
title: SP_DRVINFO_DATA_V1_W
author: windows-sdk-content
description: An SP_DRVINFO_DATA structure contains information about a driver. This structure is a member of a driver information list that can be associated with a particular device instance or globally with a device information set.
old-location: devinst\sp_drvinfo_data.htm
tech.root: devinst
ms.assetid: 13cdebad-6247-4651-a1d0-709e14af22f6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSP_DRVINFO_DATA_V1_W, PSP_DRVINFO_DATA, PSP_DRVINFO_DATA structure pointer [Device and Driver Installation], SP_DRVINFO_DATA, SP_DRVINFO_DATA structure [Device and Driver Installation], SP_DRVINFO_DATA_V1, SP_DRVINFO_DATA_V1_W, SP_DRVINFO_DATA_W, devinst.sp_drvinfo_data, di-struct_738a1fa5-729a-4464-af75-05591d68eef7.xml, setupapi/PSP_DRVINFO_DATA, setupapi/SP_DRVINFO_DATA"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: setupapi.h
req.include-header: Setupapi.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Setupapi.h
api_name:
 - SP_DRVINFO_DATA
product: Windows
targetos: Windows
req.typenames: SP_DRVINFO_DATA_V1_W, *PSP_DRVINFO_DATA_V1_W
req.redist: 
---

# SP_DRVINFO_DATA_V1_W structure


## -description


An SP_DRVINFO_DATA structure contains information about a driver. This structure is a member of a driver information list that can be associated with a particular device instance or globally with a device information set.


## -struct-fields




### -field cbSize

The size, in bytes, of the SP_DRVINFO_DATA structure. For more information, see the Remarks section in this topic.


### -field DriverType

The type of driver represented by this structure. Must be one of the following values:





#### SPDIT_CLASSDRIVER

This structure represents a class driver.



#### SPDIT_COMPATDRIVER

This structure represents a compatible driver.


### -field Reserved

Reserved. For internal use only.


### -field Description

A NULL-terminated string that describes the device supported by this driver.


### -field MfgName

A NULL-terminated string that contains the name of the manufacturer of the device supported by this driver.


### -field ProviderName

A NULL-terminated string giving the provider of this driver. This is typically the name of the organization that creates the driver or INF file. <b>ProviderName</b> can be an empty string.


#### - DriverDate

Date of the driver. From the <b>DriverVer</b> entry in the INF file. See the <a href="devinst.inf_ddinstall_section">INF DDInstall Section</a> for more information about the <b>DriverVer</b> entry.


##### - DriverType.SPDIT_CLASSDRIVER

This structure represents a class driver.


##### - DriverType.SPDIT_COMPATDRIVER

This structure represents a compatible driver.


#### - DriverVersion

Version of the driver. From the <b>DriverVer</b> entry in the INF file.


## -remarks



In <i>SetupAPI.h</i>, this structure equates to either SP_DRVINFO_DATA_V1 or SP_DRVINFO_DATA_V2, based on whether you include the following line in your source code:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>#define  USE_SP_DRVINFO_DATA_V1 1</pre>
</td>
</tr>
</table></span></div>
Define this identifier only if your component must run on Windows 98 or Millennium Edition, or on Windows NT. If your component is run only in Windows 2000 and later versions of Windows, do not define the identifier. If the identifier is not defined, SP_DRVINFO_DATA_V2 is used.

SP_DRVINFO_DATA_V1 does not contain <b>DriverDate</b> and <b>DriverVersion</b> members.

<b>SetupDi</b><i>Xxx</i> functions that take an SP_DRVINFO_DATA structure as a parameter verify that the <b>cbSize</b> member of the supplied structure is equal to the size, in bytes, of the structure. If the <b>cbSize</b> member is not set correctly for an input parameter, the function will fail and set an error code of ERROR_INVALID_PARAMETER. If the <b>cbSize</b> member is not set correctly for an output parameter, the function will fail and set an error code of ERROR_INVALID_USER_BUFFER.




## -see-also




<a href="https://msdn.microsoft.com/c4a66d0c-e9a9-41f8-87df-576795667b5c">SetupDiEnumDriverInfo</a>



<a href="https://msdn.microsoft.com/7c5b0e3f-75cd-48e1-b84e-d81e4e4db7b2">SetupDiGetDriverInstallParams</a>



<a href="https://msdn.microsoft.com/dd3d9736-755c-497c-a523-18ca66557ae7">SetupDiGetSelectedDriver</a>



<a href="https://msdn.microsoft.com/a6084bb4-f0c1-43f3-94e7-8fd0682f5ac0">SetupDiSetDriverInstallParams</a>



<a href="https://msdn.microsoft.com/791df876-9037-405b-b899-eea2b577d923">SetupDiSetSelectedDriver</a>
 

 
