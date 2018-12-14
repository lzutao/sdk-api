---
UID: NS:ntsecapi._KERB_INTERACTIVE_PROFILE
title: KERB_INTERACTIVE_PROFILE
author: windows-sdk-content
description: The KERB_INTERACTIVE_PROFILE structure contains information about an interactive logon profile. This structure is used by the LsaLogonUser function.
old-location: security\kerb_interactive_profile.htm
tech.root: secauthn
ms.assetid: 8e9dd04b-8155-4f85-be00-ff9d8297deaa
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PKERB_INTERACTIVE_PROFILE, KERB_INTERACTIVE_PROFILE, KERB_INTERACTIVE_PROFILE structure [Security], LOGON_EXTRA_SIDS, LOGON_RESOURCE_GROUPS, PKERB_INTERACTIVE_PROFILE, PKERB_INTERACTIVE_PROFILE structure pointer [Security], _lsa_kerb_interactive_profile, ntsecapi/KERB_INTERACTIVE_PROFILE, ntsecapi/PKERB_INTERACTIVE_PROFILE, security.kerb_interactive_profile"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ntsecapi.h
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
 - Ntsecapi.h
api_name:
 - KERB_INTERACTIVE_PROFILE
product: Windows
targetos: Windows
req.typenames: KERB_INTERACTIVE_PROFILE, *PKERB_INTERACTIVE_PROFILE
req.redist: 
---

# KERB_INTERACTIVE_PROFILE structure


## -description


The <b>KERB_INTERACTIVE_PROFILE</b> structure contains information about an interactive logon profile.
			

This structure is used by the <a href="https://msdn.microsoft.com/75968d53-5af2-4d77-9486-26403b73c954">LsaLogonUser</a> function.


## -struct-fields




### -field MessageType


<a href="https://msdn.microsoft.com/c590b6fd-c241-4ff8-9475-c8af7de7b431">KERB_PROFILE_BUFFER_TYPE</a> value identifying the type of logon request being made. This member can be set to <b>KerbInteractiveProfile</b>.


### -field LogonCount

Number of times the user is currently logged on.


### -field BadPasswordCount

Number of times a bad password was applied to the account since the last successful logon.


### -field LogonTime

Time when the user last logged on. This is an absolute-format standard time value.


### -field LogoffTime

Time when user should log off. This is an absolute-format standard time value.


### -field KickOffTime

Time when system should force user logoff. This is an absolute-format standard time value.


### -field PasswordLastSet

Time and date the password was last set. This is an absolute-format standard time value.


### -field PasswordCanChange

Time and date when the user can change the password. This is an absolute-format standard time value. To prevent a password from ever changing, set this member to a date very far into the future.


### -field PasswordMustChange

Time and date when the user must change the password. If the user can never change the password, this member is undefined. This is an absolute-format standard time value.


### -field LogonScript


<a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> containing the relative path to the account's logon script.


### -field HomeDirectory


<a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> containing the user's home directory.


### -field FullName


<a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> containing the user's full name.


### -field ProfilePath


<a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> containing the path to a user's roaming profile. This is used only if the user has a roaming profile.


### -field HomeDirectoryDrive


<a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> containing the drive containing the user's home directory.


### -field LogonServer


<a href="https://msdn.microsoft.com/4687d63a-4e58-4181-a48f-2724e5015e77">UNICODE_STRING</a> containing the name of the server that processed the logon request.


### -field UserFlags

Specifies how this user established the session. This can be one or more of the following flags.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="LOGON_EXTRA_SIDS"></a><a id="logon_extra_sids"></a><dl>
<dt><b>LOGON_EXTRA_SIDS</b></dt>
</dl>
</td>
<td width="60%">
The user logged on using extra <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">security identifiers</a> (SIDs).

</td>
</tr>
<tr>
<td width="40%"><a id="LOGON_RESOURCE_GROUPS"></a><a id="logon_resource_groups"></a><dl>
<dt><b>LOGON_RESOURCE_GROUPS</b></dt>
</dl>
</td>
<td width="60%">
The user logged on using a domain local group.

</td>
</tr>
</table>
 
