---
UID: NE:wuapi.tagSearchScope
title: SearchScope
author: windows-sdk-content
description: Defines the variety of updates that should be returned by the search:\_per-machine updates, per-user updates, or both.
old-location: wua\searchscope.htm
tech.root: wua_sdk
ms.assetid: a7b6a930-7b79-42dc-a4b0-da2eca0dff5c
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SearchScope, SearchScope , SearchScope enumeration [Windows Update Agent], searchScopeAllUsers, searchScopeCurrentUserOnly, searchScopeDefault, searchScopeMachineAndAllUsers, searchScopeMachineAndCurrentUser, searchScopeMachineOnly, wua.searchscope, wuapi/SearchScope, wuapi/searchScopeAllUsers, wuapi/searchScopeCurrentUserOnly, wuapi/searchScopeDefault, wuapi/searchScopeMachineAndAllUsers, wuapi/searchScopeMachineAndCurrentUser, wuapi/searchScopeMachineOnly
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: wuapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional with SP3 [desktop apps only]
req.target-min-winversvr: Windows Server 2003, Windows 2000 Server with SP3 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wuapi.idl
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
 - Wuapi.h
api_name:
 - SearchScope
product: Windows
targetos: Windows
req.typenames: SearchScope
req.redist: 
---

# SearchScope enumeration


## -description


Defines the variety of updates that should be returned by the search: per-machine updates, per-user updates, or both.


## -enum-fields




### -field searchScopeDefault

Search by using the default scope (the scope that Automatic Updates would use when searching for updates). This is currently equivalent to search ScopeMachineOnly.


### -field searchScopeMachineOnly

Search only for per-machine updates; exclude all per-user updates.


### -field searchScopeCurrentUserOnly

Search only for per-user updates applicable to the calling user – the user who owns the process which is making the Windows Update Agent (WUA) API call.


### -field searchScopeMachineAndCurrentUser

[Not currently supported.] Search for per-machine updates and for per-user updates applicable to the current user.


### -field searchScopeMachineAndAllUsers

[Not currently supported.] Search  for per-machine updates and for per-user updates applicable to any known user accounts on the computer.


### -field searchScopeAllUsers

[Not currently supported.] Search only for per-user updates applicable to any known user accounts on the computer. 


## -remarks



In versions of the Windows Update Agent that do not support per-user updates (versions that do not support the <a href="https://msdn.microsoft.com/d37017d5-6f78-4b6c-ac0b-c83b83853079">IUpdateSearcher3</a> interface), searches will always return only per-machine updates.


