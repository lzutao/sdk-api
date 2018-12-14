---
UID: NF:clusapi.ClusterSetAccountAccess
title: ClusterSetAccountAccess function
author: windows-sdk-content
description: Updates an account access list (ACL) for a cluster.
old-location: mscs\clustersetaccountaccess.htm
tech.root: mscs
ms.assetid: E0038A7B-291F-4A30-86BD-D9BD2404D3B5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: CLUSAPI_ALL_ACCESS, CLUSAPI_CHANGE_ACCESS, CLUSAPI_NO_ACCESS, CLUSAPI_READ_ACCESS, CLUSTER_DELETE_ACCESS_CONTROL_ENTRY, CLUSTER_SET_ACCESS_TYPE_ALLOWED, CLUSTER_SET_ACCESS_TYPE_DENIED, ClusterSetAccountAccess, ClusterSetAccountAccess function [Failover Cluster], PCLUSTER_SET_ACCOUNT_ACCESS, PCLUSTER_SET_ACCOUNT_ACCESS function [Failover Cluster], clusapi/ClusterSetAccountAccess, clusapi/PCLUSTER_SET_ACCOUNT_ACCESS, mscs.clustersetaccountaccess
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: clusapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2016
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: ClusAPI.lib
req.dll: ClusAPI.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - ClusAPI.dll
api_name:
 - ClusterSetAccountAccess
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ClusterSetAccountAccess function


## -description


Updates an account access list (ACL) for a cluster.


## -parameters




### -param hCluster [in]

A handle to the cluster.


### -param szAccountSID [in]

The security identifier (SID) or the account name for the new account access entry (ACE).


### -param dwAccess [in]

The access rights controlled by the ACE.


The possible values are:





#### CLUSAPI_READ_ACCESS (0x00000001L)

Read access.



#### CLUSAPI_CHANGE_ACCESS (0x00000002L)

The account can be used to make changes to the cluster.



#### CLUSAPI_NO_ACCESS (0x00000004L)

No access.



#### CLUSAPI_ALL_ACCESS ((CLUSAPI_READ_ACCESS | CLUSAPI_CHANGE_ACCESS))

The account can be used to read and change the cluster.


### -param dwControlType [in]

The  ACE type to use.


The possible values are:





#### CLUSTER_SET_ACCESS_TYPE_ALLOWED (0)

Adds an allowed ACE.



#### CLUSTER_SET_ACCESS_TYPE_DENIED (1)

Adds a denied ACE.



#### CLUSTER_DELETE_ACCESS_CONTROL_ENTRY (2)

Deletes all the ACEs for for the SID.


## -returns



If the operation succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, the function returns a 
      <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>.




## -see-also




<a href="https://msdn.microsoft.com/2bb0650f-ef9c-40bb-ae90-229bfa23838e">Cluster Registry Access Functions</a>
 

 
