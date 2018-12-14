---
UID: NS:winternl._TEB
title: TEB
author: windows-sdk-content
description: The Thread Environment Block (TEB structure) describes the state of a thread.
old-location: base\teb.htm
tech.root: procthread
ms.assetid: fc77fc09-6319-4daa-ac96-1ded661ef800
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PTEB, PTEB, PTEB structure pointer, TEB, TEB structure, base.teb, winternl/PTEB, winternl/TEB"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winternl.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Winternl.h
api_name:
 - TEB
product: Windows
targetos: Windows
req.typenames: TEB, *PTEB
req.redist: 
---

# TEB structure


## -description


<p class="CCE_Message">[This structure may be altered in future versions of Windows. Applications should use the alternate functions listed in this topic.]

The Thread Environment Block (TEB structure) describes the state of a thread.


## -struct-fields


## -remarks



The definition of this structure may change from one version of Windows to the next. Do not assume a maximum size for this structure. To see the members of this structure, refer to winternal.h.

You should not directly access this structure. To access the values of the <b>TlsSlots</b> and <b>TlsExpansionSlots</b>  members, call <a href="https://msdn.microsoft.com/82bd5ff6-ff0b-42b7-9ece-e9e8531eb5fb">TlsGetValue</a>. To access the value of the <b>ReservedForOle</b> member, call <a href="_com_cogetcontexttoken">CoGetContextToken</a>.

In the following versions of Windows, the offset of the 32-bit TEB address within the 64-bit TEB is 0. This can be used to directly access the 32-bit TEB of a WOW64 thread. This might change in later versions of Windows.

<table>
<tr>
<td>Windows Vista</td>
<td>Windows Server 2008</td>
</tr>
<tr>
<td>Windows 7</td>
<td>Windows Server 2008 R2</td>
</tr>
<tr>
<td>Windows 8</td>
<td>Windows Server 2012</td>
</tr>
<tr>
<td>Windows 8.1</td>
<td>Windows Server 2012 R2</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/82bd5ff6-ff0b-42b7-9ece-e9e8531eb5fb">TlsGetValue</a>
 

 
