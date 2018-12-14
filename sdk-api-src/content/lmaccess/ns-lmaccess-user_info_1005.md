---
UID: NS:lmaccess._USER_INFO_1005
title: USER_INFO_1005
author: windows-sdk-content
description: The USER_INFO_1005 structure contains a privilege level to assign to a user network account. This information level is valid only when you call the NetUserSetInfo function.
old-location: netmgmt\user_info_1005_str.htm
tech.root: netmgmt
ms.assetid: a953b48f-bda0-4dce-a153-d4db912de533
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPUSER_INFO_1005, *PUSER_INFO_1005, LPUSER_INFO_1005, LPUSER_INFO_1005 structure pointer [Network Management], PUSER_INFO_1005, PUSER_INFO_1005 structure pointer [Network Management], USER_INFO_1005, USER_INFO_1005 structure [Network Management], USER_PRIV_ADMIN, USER_PRIV_GUEST, USER_PRIV_USER, _win32_user_info_1005_str, lmaccess/LPUSER_INFO_1005, lmaccess/PUSER_INFO_1005, lmaccess/USER_INFO_1005, netmgmt.user_info_1005_str"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: lmaccess.h
req.include-header: Lm.h
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
 - Lmaccess.h
api_name:
 - USER_INFO_1005
product: Windows
targetos: Windows
req.typenames: USER_INFO_1005, *PUSER_INFO_1005, *LPUSER_INFO_1005
req.redist: 
---

# USER_INFO_1005 structure


## -description


The
				<b>USER_INFO_1005</b> structure contains a privilege level to assign to a user network account. This information level is valid only when you call the 
<a href="https://msdn.microsoft.com/ffe49d4b-e7e8-4982-8087-59bb7534b257">NetUserSetInfo</a> function.


## -struct-fields




### -field usri1005_priv

Specifies a <b>DWORD</b> value that indicates the level of privilege to assign for the user account specified in the <i>username</i> parameter to the 
<b>NetUserSetInfo</b> function. This member can be one of the following values. For more information about user and group account rights, see 
<a href="https://msdn.microsoft.com/fe6aae0f-93eb-4aba-a6ac-45e71c251c51">Privileges</a>. 



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="USER_PRIV_GUEST"></a><a id="user_priv_guest"></a><dl>
<dt><b>USER_PRIV_GUEST</b></dt>
</dl>
</td>
<td width="60%">
Guest

</td>
</tr>
<tr>
<td width="40%"><a id="USER_PRIV_USER"></a><a id="user_priv_user"></a><dl>
<dt><b>USER_PRIV_USER</b></dt>
</dl>
</td>
<td width="60%">
User

</td>
</tr>
<tr>
<td width="40%"><a id="USER_PRIV_ADMIN"></a><a id="user_priv_admin"></a><dl>
<dt><b>USER_PRIV_ADMIN</b></dt>
</dl>
</td>
<td width="60%">
Administrator

</td>
</tr>
</table>
 


## -see-also




<a href="https://msdn.microsoft.com/ffe49d4b-e7e8-4982-8087-59bb7534b257">NetUserSetInfo</a>



<a href="https://msdn.microsoft.com/426c7b2e-027c-4a88-97b7-eba5201d0f0d">Network Management Overview</a>



<a href="https://msdn.microsoft.com/a4b05054-bef2-4cab-89f6-725d92ee75b8">Network Management Structures</a>



<a href="https://msdn.microsoft.com/cf0e5102-3924-46c0-8124-0aa04e95f48d">User Functions</a>
 

 
