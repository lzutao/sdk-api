---
UID: NS:winnt._MESSAGE_RESOURCE_BLOCK
title: MESSAGE_RESOURCE_BLOCK
author: windows-sdk-content
description: Contains information about message strings with identifiers in the range indicated by the LowId and HighId members.
old-location: menurc\message_resource_block.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\introductiontoresources\resourcereference\resourcestructures\message_resource_block.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PMESSAGE_RESOURCE_BLOCK, MESSAGE_RESOURCE_BLOCK, MESSAGE_RESOURCE_BLOCK structure [Menus and Other Resources], _win32_MESSAGE_RESOURCE_BLOCK_str, _win32_message_resource_block_str_cpp, menurc.message_resource_block, winnt/MESSAGE_RESOURCE_BLOCK, winui._win32_message_resource_block_str"
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
 - MESSAGE_RESOURCE_BLOCK
product: Windows
targetos: Windows
req.typenames: MESSAGE_RESOURCE_BLOCK, *PMESSAGE_RESOURCE_BLOCK
req.redist: 
---

# MESSAGE_RESOURCE_BLOCK structure


## -description


Contains information about message strings with identifiers in the range indicated by the 
			<b>LowId</b> and 
			<b>HighId</b> members. 


## -struct-fields




### -field LowId

Type: <b>DWORD</b>

The lowest message identifier contained within this structure. 


### -field HighId

Type: <b>DWORD</b>

The highest message identifier contained within this structure. 


### -field OffsetToEntries

Type: <b>DWORD</b>

The offset, in bytes, from the beginning of the <a href="https://msdn.microsoft.com/439cf64e-29be-49ab-8bbf-cb98ac2e41cd">MESSAGE_RESOURCE_DATA</a> structure to the <a href="https://msdn.microsoft.com/cce13b09-5c8b-4d64-a229-419d01d91f27">MESSAGE_RESOURCE_ENTRY</a> structures in this <b>MESSAGE_RESOURCE_BLOCK</b>. The <b>MESSAGE_RESOURCE_ENTRY</b> structures contain the message strings. 


## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/439cf64e-29be-49ab-8bbf-cb98ac2e41cd">MESSAGE_RESOURCE_DATA</a>



<a href="https://msdn.microsoft.com/cce13b09-5c8b-4d64-a229-419d01d91f27">MESSAGE_RESOURCE_ENTRY</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/ff321356-c999-4021-a537-fbe863996e24">Resources</a>
 

 
