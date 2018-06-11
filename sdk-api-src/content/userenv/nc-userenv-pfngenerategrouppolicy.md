---
UID: NC:userenv.PFNGENERATEGROUPPOLICY
title: PFNGENERATEGROUPPOLICY
author: windows-sdk-content
description: The GenerateGroupPolicy callback function is an application-defined callback function that each policy extension must export when generating RSoP data in the planning mode.
old-location: policy\generategrouppolicy.htm
old-project: Policy
ms.assetid: 748b61a1-79fb-44b9-8c9b-0b1746fa981b
ms.author: windowssdkdev
ms.date: 05/30/2018
ms.keywords: GPO_INFO_FLAG_SLOWLINK, GPO_INFO_FLAG_VERBOSE, GenerateGroupPolicy, PFNGENERATEGROUPPOLICY, PFNGENERATEGROUPPOLICY callback, PFNGENERATEGROUPPOLICY callback function [Group Policy], _win32_generategrouppolicy, policy.generategrouppolicy, userenv/PFNGENERATEGROUPPOLICY
ms.prod: windows
ms.technology: windows-sdk
ms.topic: callback
req.header: userenv.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.typenames: USB_UNICODE_NAME, *PUSB_UNICODE_NAME
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - Userenv.h
api_name:
 - PFNGENERATEGROUPPOLICY
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Windows UI
---

# PFNGENERATEGROUPPOLICY callback function


## -description


The
    <b>GenerateGroupPolicy</b> callback function is an application-defined callback function that each policy extension must export when generating RSoP data in the planning mode. The Group Policy Data Access Service (GPDAS) calls the function after the service simulates the loading of client-side extensions so that extensions can generate policy data.

The <b>PFNGENERATEGROUPPOLICY</b> type defines a pointer to this callback function. 
<b>GenerateGroupPolicy</b> is a placeholder for the application-defined function name.


## -parameters




### -param dwFlags [in]

A parameter that represents one or more of the following flags.



#### GPO_INFO_FLAG_SLOWLINK

The policy is applied across a slow link.



#### GPO_INFO_FLAG_VERBOSE

Write verbose output to the event log.


### -param *pbAbort [in]

A value that specifies whether to continue processing GPOs. If this parameter is <b>TRUE</b>, GPO processing stops and the extension must deallocate its resources and return promptly. If this parameter is <b>FALSE</b>, GPO processing continues.


### -param *pwszSite [in]

A pointer to the site name of the target computer. This parameter can be <b>NULL</b>.


### -param pComputerTarget [in]

A pointer to an 
<a href="https://msdn.microsoft.com/65b0eb27-fc4a-44d6-843e-965a90dc51e8">RSOP_TARGET</a> structure that contains information about a computer. This parameter can be <b>NULL</b>, but if it is <b>NULL</b>, the <i>pUserTarget</i> parameter is required.


### -param pUserTarget [in]

A pointer to an 
<a href="https://msdn.microsoft.com/65b0eb27-fc4a-44d6-843e-965a90dc51e8">RSOP_TARGET</a> structure that contains information about a user. This parameter can be <b>NULL</b>, but if it is <b>NULL</b>, the <i>pComputerTarget</i> parameter is required.


## -returns



If the function succeeds, the return value is <b>ERROR_SUCCESS</b>. Otherwise, the function returns one of the system error codes. For a complete list of error codes, see 
<a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">System Error Codes</a> or the header file WinError.h.




## -remarks



The policy extension must register this callback function at the registry key:<b>HKEY_LOCAL_MACHINE</b>\<b>SOFTWARE</b>\<b>Microsoft</b>\<b>Windows NT</b>\<b>CurrentVersion</b>\<b>Winlogon</b>\<b>GPExtensions</b>\<b>ClientExtensionGuid</b>



<b>GenerateGroupPolicy</b>
<b>REG_SZ</b>



## -see-also




<a href="https://msdn.microsoft.com/7c45666e-d7c7-4989-ad19-b1b230757a88">Group Policy
    Functions</a>



<a href="https://msdn.microsoft.com/1285ab5a-ea68-4c16-bc34-8ab2f3cfad35">Group Policy
    Overview</a>



<a href="https://msdn.microsoft.com/65b0eb27-fc4a-44d6-843e-965a90dc51e8">RSOP_TARGET</a>
 

 
