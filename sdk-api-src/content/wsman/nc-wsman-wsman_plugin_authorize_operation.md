---
UID: NC:wsman.WSMAN_PLUGIN_AUTHORIZE_OPERATION
title: WSMAN_PLUGIN_AUTHORIZE_OPERATION
author: windows-sdk-content
description: Authorizes a specific operation.
old-location: winrm\wsman_plugin_authorize_operation.htm
tech.root: winrm
ms.assetid: 28fbd8db-557d-487b-8cf7-c550fe0826f7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: Command, Create, Delete, Enumerate, Get, Invoke, Put, Shell, Subscribe, WSMAN_PLUGIN_AUTHORIZE_OPERATION, WSMAN_PLUGIN_AUTHORIZE_OPERATION callback, WSMAN_PLUGIN_AUTHORIZE_OPERATION callback function [Windows Management Instrumentation], winrm.wsman_plugin_authorize_operation, wsman/WSMAN_PLUGIN_AUTHORIZE_OPERATION
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: wsman.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7
req.target-min-winversvr: Windows Server 2008 R2
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
 - UserDefined
api_location:
 - Wsman.h
api_name:
 - WSMAN_PLUGIN_AUTHORIZE_OPERATION
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows Management Framework on Windows Server 2008 with SP2, Windows Vista with SP1, and Windows Vista with SP2
---

# WSMAN_PLUGIN_AUTHORIZE_OPERATION callback function


## -description


Authorizes a specific operation. 

The DLL entry point name for this method must be <b>WSManPluginAuthzOperation</b>.


## -parameters




### -param pluginContext [in]

Specifies the context that was returned by a call to <a href="https://msdn.microsoft.com/b3123f52-880b-4d14-a5a2-77c5924de99d">WSManPluginStartup</a>. This parameter represents a specific application initialization of a WinRM plug-in.


### -param *senderDetails [in]

A pointer  to the <a href="https://msdn.microsoft.com/f68a9f75-6808-4dfa-b40f-061da88ead3c">WSMAN_SENDER_DETAILS</a> structure that specifies the identification information of the user.


### -param flags [in]

Reserved for future use. Must be set to zero.


### -param operation [in]

Represents the operation that is being performed. This parameter can be one of the following values:



#### Get

WSManOperationGet



#### Put

WSManOperationPut



#### Create

WSManOperationCreate



#### Delete

WSManOperationDelete



#### Enumerate

WSManOperationEnumerate



#### Subscribe

WSManOperationSubscribe



#### Shell

WSManOperationShell



#### Command

WSManOperationCommand



#### Invoke

WSManOperationInvoke


### -param action [in]

Specifies the action of the request received.  This parameter can be one of the following values:



#### Get

http://schemas.xmlsoap.org/ws/2004/09/transfer/Get



#### Put

http://schemas.xmlsoap.org/ws/2004/09/transfer/Put



#### Create

http://schemas.xmlsoap.org/ws/2004/09/transfer/Create

<div class="alert"><b>Note</b>  Shell creation will appear as Create.</div>
<div> </div>


#### Delete

http://schemas.xmlsoap.org/ws/2004/09/transfer/Delete



#### Enumerate

http://schemas.xmlsoap.org/ws/2004/09/enumeration/Enumerate



#### Subscribe

http://schemas.xmlsoap.org/ws/2004/08/eventing/Subscribe



#### Command

http://schemas.microsoft.com/wbem/wsman/1/windows/shell/Command



#### Invoke

This operation will have a custom string.


### -param resourceUri [in]

Specifies the <a href="https://msdn.microsoft.com/en-us/library/Aa384465(v=VS.85).aspx">resource URI</a> of the inbound operation.


## -returns



This callback function does not return a value.




## -remarks



The plug-in must call <a href="https://msdn.microsoft.com/1b9590ac-45d7-4eed-9477-05500c8bc1ca">WSManPluginAuthzOperationComplete</a> to report either that the user was successfully authorized to perform the operation with <b>NO_ERROR</b> or that the user was not authorized with <b>ERROR_ACCESS_DENIED</b>. All other errors report a failure to the client, but no specific information is reported.


