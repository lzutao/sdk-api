---
UID: NF:setupapi.SetupDiCreateDevRegKeyA
title: SetupDiCreateDevRegKeyA function
author: windows-sdk-content
description: The SetupDiCreateDevRegKey function creates a registry key for device-specific configuration information and returns a handle to the key.
old-location: devinst\setupdicreatedevregkey.htm
old-project: devinst
ms.assetid: 8c07db95-eb59-4e01-851d-f6a8da169625
ms.author: windowssdkdev
ms.date: 05/31/2018
ms.keywords: SetupDiCreateDevRegKey, SetupDiCreateDevRegKey function [Device and Driver Installation], SetupDiCreateDevRegKeyA, SetupDiCreateDevRegKeyW, devinst.setupdicreatedevregkey, di-rtns_284367d1-6053-4fd1-990b-7028a116ece2.xml, setupapi/SetupDiCreateDevRegKey
ms.prod: windows
ms.technology: windows-sdk
ms.topic: function
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
tech.root: 
req.typenames: TSSD_ConnectionPoint, *PTSSD_ConnectionPoint
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - Setupapi.lib
 - Setupapi.dll
api_name:
 - SetupDiCreateDevRegKey
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# SetupDiCreateDevRegKeyA function


## -description


The <b>SetupDiCreateDevRegKey</b> function creates a registry key for device-specific configuration information and returns a handle to the key. 


## -parameters




### -param DeviceInfoSet [in]

A handle to a <a href="devinst.device_information_sets">device information set</a> that contains a device information element that represents the device for which to create a registry key. 


### -param DeviceInfoData [in]

A pointer to an <a href="https://msdn.microsoft.com/library/windows/hardware/ff552344">SP_DEVINFO_DATA</a> structure that specifies the device information element in <i>DeviceInfoSet</i>.


### -param Scope [in]

The scope of the registry key to be created. The scope determines where the information is stored. The key created can be global or hardware profile-specific. Can be one of the following values:





#### DICS_FLAG_GLOBAL

Create a key to store global configuration information. This information is not specific to a particular hardware profile. On NT-based operating systems this creates a key that is rooted at <b>HKEY_LOCAL_MACHINE</b>. The exact key opened depends on the value of the <i>KeyType</i> parameter.



#### DICS_FLAG_CONFIGSPECIFIC

Create a key to store hardware profile-specific configuration information. This key is rooted at one of the hardware-profile specific branches, instead of <b>HKEY_LOCAL_MACHINE</b>.


### -param HwProfile [in]

The hardware profile for which to create a key if <i>HwProfileFlags</i> is set to SPDICS_FLAG_CONFIGSPECIFIC. If <i>HwProfile</i> is 0, the key for the current hardware profile is created. If <i>HwProfileFlags</i> is SPDICS_FLAG_GLOBAL, <i>HwProfile</i> is ignored.


### -param KeyType [in]

The type of registry storage key to create. Can be one of the following values:





#### DIREG_DEV

Create a <a href="https://msdn.microsoft.com/3be5c842-d1b6-4c34-8990-e23e2d08dd23">hardware key</a> for the device. 



#### DIREG_DRV

Create a <a href="https://msdn.microsoft.com/5f6fec1a-1134-4765-81be-9b50939e5e66">software key</a> for the device.


### -param InfHandle [in, optional]

The handle to an open INF file that contains an <a href="devinst.inf_ddinstall_section">INF DDInstall section</a> to be executed for the newly created key. This parameter is optional and can be <b>NULL</b>. If this parameter is specified, <i>InfSectionName</i> must be specified as well.


### -param InfSectionName [in, optional]

The name of an INF <i>DDInstall</i> section in the INF file specified by <i>InfHandle</i>. This section is executed for the newly created key. This parameter is optional and can be <b>NULL</b>. If this parameter is specified, <i>InfHandle</i> must be specified as well.


## -returns



If <b>SetupDiCreateDevRegKey</b> succeeds, the function returns a handle to the specified registry key in which device-specific configuration data can be stored and retrieved. If <b>SetupDiCreateDevRegKey</b> fails, the function returns INVALID_HANDLE_VALUE. Call <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a> to get extended error information.




## -remarks



The caller of <b>SetupDiCreateDevRegKey</b> must be a member of the Administrators group.

Close the handle returned from <b>SetupDiCreateDevRegKey</b> by calling <a href="http://go.microsoft.com/fwlink/p/?linkid=194543">RegCloseKey</a>.

If the specified key already exists, <b>SetupDiCreateDevRegKey</b> returns a handle to that key. Otherwise, <b>SetupDiCreateDevRegKey</b> creates the specified key and returns a handle to the new key. For Windows Server 2003 and later versions of Windows, the key handle has KEY_READ and KEY_WRITE access only. For previous Windows versions, this handle has KEY_ALL_ACCESS access. 

The specified device instance must be registered before <b>SetupDiCreateDevRegKey</b> is called. Note, however, that the operating system automatically registers PnP device instances. For information about how to register non-PnP device instances, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff552091">SetupDiRegisterDeviceInfo</a>.

For installations that use layout files (specified by the <b>LayoutFile</b> entry in an <a href="https://msdn.microsoft.com/53e30950-28a3-4ae3-a351-a917b02c84a5">INF Version section</a>), the layout file must be opened by a call to <b>SetupOpenAppendInfFile</b> (described in the Microsoft Windows SDK documentation) before <b>SetupDiCreateDevRegKey</b> is called.

If the supplied device information set contains device information elements for a remote system, and <i>InfHandle</i> and <i>InfSectionName</i> are also specified, the create request will fail, and a subsequent call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a> will return ERROR_REMOTE_REQUEST_UNSUPPORTED.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff550952">SetupDiCreateDeviceInfo</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551997">SetupDiGetHwProfileList</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552079">SetupDiOpenDevRegKey</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552091">SetupDiRegisterDeviceInfo</a>
 

 
