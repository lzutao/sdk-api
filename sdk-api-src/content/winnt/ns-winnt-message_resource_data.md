---
UID: NS:winnt._MESSAGE_RESOURCE_DATA
title: MESSAGE_RESOURCE_DATA
author: windows-sdk-content
description: Contains information about formatted text for display as an error message or in a message box in a message table resource.
old-location: menurc\message_resource_data.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\introductiontoresources\resourcereference\resourcestructures\message_resource_data.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PMESSAGE_RESOURCE_DATA, MESSAGE_RESOURCE_DATA, MESSAGE_RESOURCE_DATA structure [Menus and Other Resources], PMESSAGE_RESOURCE_DATA, PMESSAGE_RESOURCE_DATA structure pointer [Menus and Other Resources], _win32_MESSAGE_RESOURCE_DATA_str, _win32_message_resource_data_str_cpp, menurc.message_resource_data, winnt/MESSAGE_RESOURCE_DATA, winnt/PMESSAGE_RESOURCE_DATA, winui._win32_message_resource_data_str"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winnt.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
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
 - Winnt.h
api_name:
 - MESSAGE_RESOURCE_DATA
product: Windows
targetos: Windows
req.typenames: MESSAGE_RESOURCE_DATA, *PMESSAGE_RESOURCE_DATA
req.redist: 
---

# MESSAGE_RESOURCE_DATA structure


## -description


Contains information about formatted text for display as an error message or in a message box in a message table resource. 


## -struct-fields




### -field NumberOfBlocks

Type: <b>DWORD</b>

The number of <a href="https://msdn.microsoft.com/573f22be-d204-4c0d-9c45-bd6d46094e32">MESSAGE_RESOURCE_BLOCK</a> structures. 


### -field Blocks

Type: <b><a href="https://msdn.microsoft.com/573f22be-d204-4c0d-9c45-bd6d46094e32">MESSAGE_RESOURCE_BLOCK</a>[1]</b>

An array of structures. The array is the size indicated by the 
					<b>NumberOfBlocks</b>  member. 


## -remarks



A <b>MESSAGE_RESOURCE_DATA</b> structure can contain one or more 
				<a href="https://msdn.microsoft.com/573f22be-d204-4c0d-9c45-bd6d46094e32">MESSAGE_RESOURCE_BLOCK</a> structures, which can each contain one or more <a href="https://msdn.microsoft.com/cce13b09-5c8b-4d64-a229-419d01d91f27">MESSAGE_RESOURCE_ENTRY</a> structures. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/573f22be-d204-4c0d-9c45-bd6d46094e32">MESSAGE_RESOURCE_BLOCK</a>



<a href="https://msdn.microsoft.com/cce13b09-5c8b-4d64-a229-419d01d91f27">MESSAGE_RESOURCE_ENTRY</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/ff321356-c999-4021-a537-fbe863996e24">Resources</a>
 

 
