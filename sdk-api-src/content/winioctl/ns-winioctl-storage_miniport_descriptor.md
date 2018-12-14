---
UID: NS:winioctl._STORAGE_MINIPORT_DESCRIPTOR
title: STORAGE_MINIPORT_DESCRIPTOR
author: windows-sdk-content
description: Reserved for system use.
old-location: fs\storage_miniport_descriptor.htm
tech.root: fileio
ms.assetid: b962666d-60ae-4e0b-813e-7b22e1670644
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSTORAGE_MINIPORT_DESCRIPTOR, PSTORAGE_MINIPORT_DESCRIPTOR, PSTORAGE_MINIPORT_DESCRIPTOR structure pointer [Files], STORAGE_MINIPORT_DESCRIPTOR, STORAGE_MINIPORT_DESCRIPTOR structure [Files], StoragePortCodeSetReserved, StoragePortCodeSetSCSIport, StoragePortCodeSetStorport, fs.storage_miniport_descriptor, winioctl/PSTORAGE_MINIPORT_DESCRIPTOR, winioctl/STORAGE_MINIPORT_DESCRIPTOR"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winioctl.h
req.include-header: Windows.h
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
 - WinIoCtl.h
api_name:
 - STORAGE_MINIPORT_DESCRIPTOR
product: Windows
targetos: Windows
req.typenames: STORAGE_MINIPORT_DESCRIPTOR, *PSTORAGE_MINIPORT_DESCRIPTOR
req.redist: 
---

# STORAGE_MINIPORT_DESCRIPTOR structure


## -description


Reserved for system use.


## -struct-fields




### -field Version

Contains the size of this structure, in bytes. The value of this member will change as members are added to 
      the structure.


### -field Size

Specifies the total size of the data returned, in bytes. This may include data that follows this 
      structure.


### -field Portdriver

Type of port driver as enumerated by the 
     <a href="https://msdn.microsoft.com/1c1032e8-30b8-45ad-973a-c7616139b26e">STORAGE_PORT_CODE_SET</a> enumeration.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="StoragePortCodeSetReserved"></a><a id="storageportcodesetreserved"></a><a id="STORAGEPORTCODESETRESERVED"></a><dl>
<dt><b>StoragePortCodeSetReserved</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
Indicates an unknown storage adapter driver type.

</td>
</tr>
<tr>
<td width="40%"><a id="StoragePortCodeSetStorport"></a><a id="storageportcodesetstorport"></a><a id="STORAGEPORTCODESETSTORPORT"></a><dl>
<dt><b>StoragePortCodeSetStorport</b></dt>
<dt>1</dt>
</dl>
</td>
<td width="60%">
Storage adapter driver is a Storport-miniport driver.

</td>
</tr>
<tr>
<td width="40%"><a id="StoragePortCodeSetSCSIport"></a><a id="storageportcodesetscsiport"></a><a id="STORAGEPORTCODESETSCSIPORT"></a><dl>
<dt><b>StoragePortCodeSetSCSIport</b></dt>
<dt>2</dt>
</dl>
</td>
<td width="60%">
Storage adapter driver is a SCSI Port-miniport driver.

</td>
</tr>
</table>
 


### -field LUNResetSupported

Indicates whether a LUN reset is supported.


### -field TargetResetSupported

Indicates whether a target reset is supported.


### -field IoTimeoutValue

 


### -field ExtraIoInfoSupported

 


### -field Reserved0

 


### -field Reserved1

 




## -see-also




<a href="https://msdn.microsoft.com/dd55c570-68b5-4dc5-9fd0-a6e3277c318b">Disk Management Structures</a>



<a href="https://msdn.microsoft.com/1c1032e8-30b8-45ad-973a-c7616139b26e">STORAGE_PORT_CODE_SET</a>
 

 
