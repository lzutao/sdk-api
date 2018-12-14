---
UID: NF:resapi.ResUtilGetResourceDependencyByClassEx
title: ResUtilGetResourceDependencyByClassEx function
author: windows-sdk-content
description: Enumerates the dependencies of a specified resource in a specified cluster and returns a handle to a dependency that matches a specified resource class. The PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_CLASS_EX type defines a pointer to this function.
old-location: mscs\resutilgetresourcedependencybyclassex.htm
tech.root: mscs
ms.assetid: D35816C8-A449-41FF-9398-A6A4E19C29FB
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_CLASS_EX, PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_CLASS_EX function [Failover Cluster], ResUtilGetResourceDependencyByClassEx, ResUtilGetResourceDependencyByClassEx function [Failover Cluster], mscs.resutilgetresourcedependencybyclassex, resapi/PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_CLASS_EX, resapi/ResUtilGetResourceDependencyByClassEx
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: resapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: ResUtils.lib
req.dll: ResUtils.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - ResUtils.dll
api_name:
 - ResUtilGetResourceDependencyByClassEx
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ResUtilGetResourceDependencyByClassEx function


## -description


Enumerates the  <a href="https://msdn.microsoft.com/2ad913d2-99cb-4885-a1de-822f77dc2030">dependencies</a> of a specified  <a href="https://msdn.microsoft.com/090d1c20-fab3-43dd-bfe2-a2c3f9ba8f89">resource</a> in a specified <a href="https://msdn.microsoft.com/en-us/library/Aa369336(v=VS.85).aspx">cluster</a> and returns a handle to a dependency that matches a specified resource class. The <b>PRESUTIL_GET_RESOURCE_DEPENDENCY_BY_CLASS_EX</b> type defines a pointer to this function.


## -parameters




### -param hCluster [in]

A handle to the cluster to which the resource belongs.


### -param hSelf [in]

A handle to the dependent resource. This resource depends on one or more resources.


### -param prci [in]

A pointer to a  <a href="https://msdn.microsoft.com/b8b6c479-2e35-4cc9-b864-d495c3bded25">PCLUS_RESOURCE_CLASS_INFO</a> structure that describes  the resource class of the dependency to return.


### -param bRecurse [in]

Determines the scope of the search. If <b>TRUE</b>, the function checks the entire dependency tree under the dependent resource. If <b>FALSE</b>, the function checks only the resources on which the dependent resource directly depends.


### -param dwDesiredAccess [in]

The requested access privileges. This  might be any combination of <b>GENERIC_READ</b> (0x80000000), <b>GENERIC_ALL</b> (0x10000000), or <b>MAXIMUM_ALLOWED</b> (0x02000000). If this value is zero (0), an undefined error  might be returned. Using <b>GENERIC_ALL</b> is the same as calling <a href="https://msdn.microsoft.com/7c2bd24a-8034-4a5f-8218-0a23d5e29b07">ResUtilGetResourceDependencyByClass</a>.


## -returns



If the operation succeeds, 
the function returns a handle to one of the resources on which the resource that is specified by <i>hSelf</i> depends. The caller is responsible for closing the handle by calling  <a href="https://msdn.microsoft.com/dbefd7f9-3499-45b3-a5c8-d0000632f61c">CloseClusterResource</a>.

If the operation fails, the function returns <b>NULL</b>. For more information, call the   <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> function.




## -see-also




<a href="https://msdn.microsoft.com/42eb7c1b-6bd6-4997-b33e-ed16470c8475">Resource Utility Functions</a>
 

 
