---
UID: NS:ipmib._MIB_MFE_TABLE
title: MIB_MFE_TABLE
author: windows-sdk-content
description: Contains a table of Multicast Forwarding Entries (MFEs).
old-location: mib\mib_mfe_table.htm
tech.root: MIB
ms.assetid: 2567e899-760d-41dd-8347-634c1a0e5764
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PMIB_MFE_TABLE, MIB_MFE_TABLE, MIB_MFE_TABLE structure [MIB], PMIB_MFE_TABLE, PMIB_MFE_TABLE structure pointer [MIB], _mpr_mib_mfe_table, ipmib/MIB_MFE_TABLE, ipmib/PMIB_MFE_TABLE, iprtrmib/MIB_MFE_TABLE, iprtrmib/PMIB_MFE_TABLE, mib.mib_mfe_table, rras.mib_mfe_table"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ipmib.h
req.include-header: Iphlpapi.h
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - Ipmib.h
 - Iprtrmib.h
api_name:
 - MIB_MFE_TABLE
product: Windows
targetos: Windows
req.typenames: MIB_MFE_TABLE, *PMIB_MFE_TABLE
req.redist: 
---

# MIB_MFE_TABLE structure


## -description


The 
<b>MIB_MFE_TABLE</b> structure contains a table of Multicast Forwarding Entries (MFEs).


## -struct-fields




### -field dwNumEntries

The number of MFEs in the table.


### -field table

A pointer to a table of MFEs implemented as an array of 
<a href="https://msdn.microsoft.com/731e2c88-5c4f-4165-a9f2-287b4c10c76b">MIB_IPMCAST_MFE</a> structures.


## -remarks



On the Microsoft Windows Software Development Kit (SDK) released for Windows Server 2008and later, the organization of header files has changed. This  structure is defined in the <i>Ipmib.h</i> header file, not in the <i>Iprtrmib.h</i> header file. Note that the <i>Ipmib.h</i> header file is automatically included in <i>Iprtrmib.h</i>, which is automatically included in the <i>Iphlpapi.h</i> header file. The  <i>Ipmib.h</i> and <i>Iprtrmib.h</i> header files should never be used directly.




## -see-also




<a href="https://msdn.microsoft.com/731e2c88-5c4f-4165-a9f2-287b4c10c76b">MIB_IPMCAST_MFE</a>
 

 
