---
UID: NF:setupapi.SetupDiSetClassRegistryPropertyW
title: SetupDiSetClassRegistryPropertyW function
author: windows-sdk-content
description: The SetupDiSetClassRegistryProperty function sets a specified device class property in the registry.
old-location: devinst\setupdisetclassregistryproperty.htm
old-project: devinst
ms.assetid: 78457461-11ef-44ec-aa60-1adf4a48db8c
ms.author: windowssdkdev
ms.date: 05/31/2018
ms.keywords: SetupDiSetClassRegistryProperty, SetupDiSetClassRegistryProperty function [Device and Driver Installation], SetupDiSetClassRegistryPropertyA, SetupDiSetClassRegistryPropertyW, devinst.setupdisetclassregistryproperty, di-rtns_77b5fc07-42ec-4515-b20c-87cf1c8e4b86.xml, setupapi/SetupDiSetClassRegistryProperty
ms.prod: windows
ms.technology: windows-sdk
ms.topic: function
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Windows XP and later versions of Windows.
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
 - SetupDiSetClassRegistryProperty
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# SetupDiSetClassRegistryPropertyW function


## -description


The <b>SetupDiSetClassRegistryProperty</b> function sets a specified device class property in the registry.


## -parameters




### -param ClassGuid [in]

A pointer to the GUID that identifies the device class for which a property is to be set.


### -param Property [in]

A value that identifies the property to be set, which must be one of the following:





#### SPCRP_CHARACTERISTICS

The caller supplies flags  that specify the device characteristics for the class. For a list of characteristics flags, see the <i>DeviceCharacteristics</i> parameter of <a href="https://msdn.microsoft.com/library/windows/hardware/ff548397">IoCreateDevice</a>. Device characteristics should be set when the device class is installed and should not be changed after the device class is installed.



#### SPCRP_DEVTYPE

The caller supplies the device type for the class. For more information, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff563821">Specifying Device Types</a>. Device type should be set when a device class is installed and should not be changed after the device class is installed.



#### SPCRP_EXCLUSIVE

The caller supplies a DWORD value  that specifies whether users can obtain exclusive access to devices for this class. The supplied value is 1 if exclusive access is allowed, or zero otherwise. The exclusive setting for a device should be set when a device class is installed and should not be changed after the device class is installed.



#### SPCRP_LOWERFILTERS

(Windows Vista and later) The caller supplies a REG_MULTI_SZ list of the service names of the lower filter drivers that are installed for the <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff552344">device setup class</a>. For more information about how to install a class filter driver, see <a href="devinst.installing_a_filter_driver">Installing a Filter Driver</a> and <a href="devinst.inf_classinstall32_section">INF ClassInstall32 Section</a>. 



#### SPCRP_SECURITY

The caller supplies the device's security descriptor as a SECURITY_DESCRIPTOR structure in self-relative format (described in the Microsoft Windows SDK documentation).



#### SPCRP_SECURITY_SDS

The caller supplies the device's security descriptor as a text string. For information about security descriptor strings, see <a href="https://msdn.microsoft.com/2b15325e-34ed-497b-ae6d-3ec3ac168232">Security Descriptor Definition Language (Windows)</a>. For information about the format of security descriptor strings, see Security Descriptor Definition Language (Windows).



#### SPCRP_UPPERFILTERS

(Windows Vista and later) The caller supplies a REG_MULTI_SZ list of the service names of the upper filter drivers that are installed for the device setup class. For more information about how to install a class filter driver, see <a href="devinst.installing_a_filter_driver">Installing a Filter Driver</a> and <a href="devinst.inf_classinstall32_section">INF ClassInstall32 Section</a>. 


### -param PropertyBuffer [in, optional]

A pointer to a buffer that supplies the specified property. This parameter is optional and can be <b>NULL</b>.


### -param PropertyBufferSize [in]

The size, in bytes, of the <i>PropertyBuffer </i>buffer.


### -param MachineName [in, optional]

A pointer to a NULL-terminated string that contains the name of a remote system on which to set the specified device class property. This parameter is optional and can be <b>NULL</b>. If this parameter is <b>NULL</b>, the property is set on the name of the local system.


### -param Reserved

Reserved, must be <b>NULL</b>.


##### - Property.SPCRP_CHARACTERISTICS

The caller supplies flags  that specify the device characteristics for the class. For a list of characteristics flags, see the <i>DeviceCharacteristics</i> parameter of <a href="https://msdn.microsoft.com/library/windows/hardware/ff548397">IoCreateDevice</a>. Device characteristics should be set when the device class is installed and should not be changed after the device class is installed.


##### - Property.SPCRP_DEVTYPE

The caller supplies the device type for the class. For more information, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff563821">Specifying Device Types</a>. Device type should be set when a device class is installed and should not be changed after the device class is installed.


##### - Property.SPCRP_EXCLUSIVE

The caller supplies a DWORD value  that specifies whether users can obtain exclusive access to devices for this class. The supplied value is 1 if exclusive access is allowed, or zero otherwise. The exclusive setting for a device should be set when a device class is installed and should not be changed after the device class is installed.


##### - Property.SPCRP_LOWERFILTERS

(Windows Vista and later) The caller supplies a REG_MULTI_SZ list of the service names of the lower filter drivers that are installed for the <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff552344">device setup class</a>. For more information about how to install a class filter driver, see <a href="devinst.installing_a_filter_driver">Installing a Filter Driver</a> and <a href="devinst.inf_classinstall32_section">INF ClassInstall32 Section</a>. 


##### - Property.SPCRP_SECURITY

The caller supplies the device's security descriptor as a SECURITY_DESCRIPTOR structure in self-relative format (described in the Microsoft Windows SDK documentation).


##### - Property.SPCRP_SECURITY_SDS

The caller supplies the device's security descriptor as a text string. For information about security descriptor strings, see <a href="https://msdn.microsoft.com/2b15325e-34ed-497b-ae6d-3ec3ac168232">Security Descriptor Definition Language (Windows)</a>. For information about the format of security descriptor strings, see Security Descriptor Definition Language (Windows).


##### - Property.SPCRP_UPPERFILTERS

(Windows Vista and later) The caller supplies a REG_MULTI_SZ list of the service names of the upper filter drivers that are installed for the device setup class. For more information about how to install a class filter driver, see <a href="devinst.installing_a_filter_driver">Installing a Filter Driver</a> and <a href="devinst.inf_classinstall32_section">INF ClassInstall32 Section</a>. 


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved with a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



The caller of this function must be a member of the Administrators group.

To determine the data type for a device class property, call <a href="https://msdn.microsoft.com/library/windows/hardware/ff551097">SetupDiGetClassRegistryProperty</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff551097">SetupDiGetClassRegistryProperty</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551967">SetupDiGetDeviceRegistryProperty</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552169">SetupDiSetDeviceRegistryProperty</a>
 

 
