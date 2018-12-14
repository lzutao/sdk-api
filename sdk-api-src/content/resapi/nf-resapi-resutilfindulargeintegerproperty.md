---
UID: NF:resapi.ResUtilFindULargeIntegerProperty
title: ResUtilFindULargeIntegerProperty function
author: windows-sdk-content
description: Gets a large integer property value from a property list. The PRESUTIL_FIND_ULARGEINTEGER_PROPERTY type defines a pointer to this function.
old-location: mscs\resutilfindulargeintegerproperty.htm
tech.root: mscs
ms.assetid: BA4DD6F0-07DB-4601-B8EB-E79B49F2829F
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PRESUTIL_FIND_ULARGEINTEGER_PROPERTY, PRESUTIL_FIND_ULARGEINTEGER_PROPERTY function [Failover Cluster], ResUtilFindULargeIntegerProperty, ResUtilFindULargeIntegerProperty function [Failover Cluster], mscs.resutilfindulargeintegerproperty, resapi/PRESUTIL_FIND_ULARGEINTEGER_PROPERTY, resapi/ResUtilFindULargeIntegerProperty
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: resapi.h
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
 - ResUtilFindULargeIntegerProperty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ResUtilFindULargeIntegerProperty function


## -description


Gets a large integer property value from a property list. The <b>PRESUTIL_FIND_ULARGEINTEGER_PROPERTY</b> type defines a pointer to this function.


## -parameters




### -param pPropertyList [in]

A pointer to the property list.


### -param cbPropertyListSize [in]

The size of the data in <i>pPropertyList</i>, in bytes.


### -param pszPropertyName [in]

The name of the property.


### -param plPropertyValue [out]

The value of the property.


## -returns



If the operations succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, the function returns a 
       <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>. The following is a possible error 
       code.




## -see-also




<a href="https://msdn.microsoft.com/b6287135-e9b3-43ab-aaf4-1488dad3e9ed">Property List Parsing Functions</a>
 

 
