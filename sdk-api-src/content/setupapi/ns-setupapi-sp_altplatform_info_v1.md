---
UID: NS:setupapi._SP_ALTPLATFORM_INFO_V1
title: SP_ALTPLATFORM_INFO_V1
author: windows-sdk-content
description: This structure is used to pass information for an alternate platform to SetupQueryInfOriginalFileInformation.
old-location: setup\sp_altplatform_info_v1.htm
tech.root: SetupApi
ms.assetid: 33872a84-8f7f-4508-a326-2d95ac0fcfd7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSP_ALTPLATFORM_INFO_V1, PSP_ALTPLATFORM_INFO_V1, PSP_ALTPLATFORM_INFO_V1 structure pointer [Setup API], SP_ALTPLATFORM_INFO, SP_ALTPLATFORM_INFO_V1, SP_ALTPLATFORM_INFO_V1 structure [Setup API], VER_PLATFORM_WIN32_NT, VER_PLATFORM_WIN32_WINDOWS, _setupapi_sp_altplatform_info, setup.sp_altplatform_info_v1, setupapi/PSP_ALTPLATFORM_INFO_V1, setupapi/SP_ALTPLATFORM_INFO_V1"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: setupapi.h
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
 - Setupapi.h
api_name:
 - SP_ALTPLATFORM_INFO_V1
product: Windows
targetos: Windows
req.typenames: SP_ALTPLATFORM_INFO_V1, *PSP_ALTPLATFORM_INFO_V1
req.redist: 
---

# SP_ALTPLATFORM_INFO_V1 structure


## -description


This structure is used to pass information for an alternate platform to 
<a href="https://msdn.microsoft.com/bc7c08ff-3d6b-4d45-b634-1358302f6fc6">SetupQueryInfOriginalFileInformation</a>.

Setup implicitly uses the <b>SP_ALTPLATFORM_INFO_V1</b> structure if USE_SP_ALTPLATFORM_INFO_V1 is set to 1 or if _WIN32_WINNT is less than or equal to 0x500. This version is for use with Windows 2000.

Setup implicitly uses the <a href="https://msdn.microsoft.com/eb66ef5a-212d-4224-87b5-d64e8e188139">SP_ALTPLATFORM_INFO_V2</a> structure if USE_SP_ALTPLATFORM_INFO_V1 is 0 or undefined and _WIN32_WINNT is set to 0x501. 


## -struct-fields




### -field cbSize

Size of this structure, in bytes.


### -field Platform

Operating system. This must be one of the following values. 



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="VER_PLATFORM_WIN32_WINDOWS"></a><a id="ver_platform_win32_windows"></a><dl>
<dt><b>VER_PLATFORM_WIN32_WINDOWS</b></dt>
</dl>
</td>
<td width="60%">
Legacy operating systems.

</td>
</tr>
<tr>
<td width="40%"><a id="VER_PLATFORM_WIN32_NT"></a><a id="ver_platform_win32_nt"></a><dl>
<dt><b>VER_PLATFORM_WIN32_NT</b></dt>
</dl>
</td>
<td width="60%">
Windows Server 2008, Windows Vista, Windows Server 2003, Windows XP, or Windows 2000.

</td>
</tr>
</table>
 


### -field MajorVersion

Major version of the operating system.


### -field MinorVersion

Minor version of the operating system.


### -field ProcessorArchitecture

Processor architecture. This must be PROCESSOR_ARCHITECTURE_INTEL, PROCESSOR_ARCHITECTURE_ALPHA, PROCESSOR_ARCHITECTURE_IA64, PROCESSOR_ARCHITECTURE_ALPHA64.


### -field Reserved

Must be set to zero.


## -see-also




<a href="https://msdn.microsoft.com/58201596-cb8c-480a-abef-896c1f9ef098">Overview</a>



<a href="https://msdn.microsoft.com/eb66ef5a-212d-4224-87b5-d64e8e188139">SP_ALTPLATFORM_INFO_V2</a>



<a href="https://msdn.microsoft.com/837F1864-CE2F-4A9A-A7D9-18EB8622541E">Structures</a>
 

 
