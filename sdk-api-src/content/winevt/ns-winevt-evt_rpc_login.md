---
UID: NS:winevt._EVT_RPC_LOGIN
title: EVT_RPC_LOGIN
author: windows-sdk-content
description: Contains the information used to connect to a remote computer.
old-location: wes\evt_rpc_login.htm
tech.root: wes
ms.assetid: 38f74619-1643-461f-b04b-c15567c06ca8
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: EVT_RPC_LOGIN, EVT_RPC_LOGIN structure [EventLog], wes.evt_rpc_login, winevt/_EVT_RPC_LOGIN
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winevt.h
req.include-header: 
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
 - WinEvt.h
api_name:
 - EVT_RPC_LOGIN
product: Windows
targetos: Windows
req.typenames: EVT_RPC_LOGIN
req.redist: 
---

# EVT_RPC_LOGIN structure


## -description


Contains the information used to connect to a remote computer.


## -struct-fields




### -field Server

The name of the remote computer to connect to.


### -field User

The user name to use to connect to the remote computer.


### -field Domain

The domain to which the user account belongs. Optional.


### -field Password

The password for the user account.


### -field Flags

The authentication method to use to authenticate the user when connecting to the remote computer. For possible authentication methods, see the <a href="https://msdn.microsoft.com/f3001756-7c2d-4a96-bbdf-e707debb5374">EVT_RPC_LOGIN_FLAGS</a> enumeration. 


## -remarks



You can set <b>User</b>, <b>Domain</b>, and <b>Password</b> to <b>NULL</b> to use the credentials of the current user.

If you set <b>Password</b>, consider using the <a href="https://msdn.microsoft.com/2c4090a6-025b-4b7b-8f31-7e744ad51b39">SecureZeroMemory</a> function to clear the password after calling <a href="https://msdn.microsoft.com/26f1745c-dcca-4452-872e-1fffe20f049c">EvtOpenSession</a>.




## -see-also




<a href="https://msdn.microsoft.com/26f1745c-dcca-4452-872e-1fffe20f049c">EvtOpenSession</a>
 

 
