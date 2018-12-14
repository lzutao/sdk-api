---
UID: NS:tspubplugincom.__MIDL_ItsPubPlugin_0001
title: pluginResource
author: windows-sdk-content
description: Contains information about a resource that can be assigned to users in RemoteApp and Desktop Connection.
old-location: termserv\pluginresource.htm
tech.root: TermServ
ms.assetid: 209dee74-c52e-4e31-9d1b-1e7c6c0d0121
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: pluginResource, pluginResource structure [Remote Desktop Services], termserv.pluginresource, tspubplugincom/pluginResource
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: tspubplugincom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Cpubplugin.idl
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
 - tspubplugincom.h
api_name:
 - pluginResource
product: Windows
targetos: Windows
req.typenames: pluginResource
req.redist: 
---

# pluginResource structure


## -description


Contains information about a resource that can be assigned to users in RemoteApp and Desktop Connection.


## -struct-fields




### -field alias

The  alias of the resource.


### -field name

The  name of the resource.


### -field resourceFileContents

The contents of the resource file. The plug-in should allocate memory for this member by calling the <a href="https://msdn.microsoft.com/c4cb588d-9482-4f90-a92e-75b604540d5c">CoTaskMemAlloc</a> function.


### -field fileExtension

The file name extension of the resource file. If this member is set to ".rdp", RD Web Access opens the file by using the ActiveX control.


### -field resourcePluginType

A unique identifier that identifies the resource plug-in.


### -field isDiscoverable

A Boolean value that indicates whether the resource should be displayed in RD Web Access or RemoteApp and Desktop Connections.


### -field resourceType

The type of resource.



#### 1

RemoteApp application.



#### 2

Personal virtual desktop.


### -field pceIconSize

The size, in bytes, of the icon.


### -field iconContents

A byte array that defines the icon to be displayed for the resource.


### -field pcePluginBlobSize

The size, in bytes, of the <b>blobContents</b> member.


### -field blobContents

This member is reserved. Set it to <b>NULL</b>.


## -see-also




<a href="https://msdn.microsoft.com/bd928bdc-e4b4-4b5a-a782-0881ed6d08bd">RemoteApp and Desktop Connection Management Service Interfaces</a>



<a href="https://msdn.microsoft.com/4295bd3c-0fc9-4135-b9cc-cafbc8381797">RemoteApp and Desktop Connection Management Service Structures</a>
 

 
