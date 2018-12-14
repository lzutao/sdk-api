---
UID: NF:resapi.ResUtilFindMultiSzProperty
title: ResUtilFindMultiSzProperty function
author: windows-sdk-content
description: Locates a multiple string property in a property list. The PRESUTIL_FIND_MULTI_SZ_PROPERTY type defines a pointer to this function.
old-location: mscs\resutilfindmultiszproperty.htm
tech.root: mscs
ms.assetid: 65209ca8-e293-40cc-ac8a-9643933e049f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PRESUTIL_FIND_MULTI_SZ_PROPERTY, PRESUTIL_FIND_MULTI_SZ_PROPERTY function [Failover Cluster], ResUtilFindMultiSzProperty, ResUtilFindMultiSzProperty function [Failover Cluster], _wolf_resutilfindmultiszproperty, mscs.resutilfindmultiszproperty, resapi/PRESUTIL_FIND_MULTI_SZ_PROPERTY, resapi/ResUtilFindMultiSzProperty
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: resapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Enterprise, Windows Server 2008 Datacenter
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
 - ResUtilFindMultiSzProperty
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ResUtilFindMultiSzProperty function


## -description


Locates a multiple string property in a  <a href="https://msdn.microsoft.com/57312b32-01cf-48e8-b61f-6095e23bb580">property list</a>. The <b>PRESUTIL_FIND_MULTI_SZ_PROPERTY</b> type defines a pointer to this function.


## -parameters




### -param pPropertyList [in]

Pointer to the property list in which to locate the value.


### -param cbPropertyListSize [in]

Size in bytes of the data included in <i>pPropertyList</i>.


### -param pszPropertyName [in]

Pointer to a null-terminated Unicode string containing the name of the value to locate.


### -param pszPropertyValue [out]

Pointer to a <b>WCHAR</b> pointer to a buffer (allocated by the function) containing a copy of the property value. You must call <a href="https://msdn.microsoft.com/a0393983-cb43-4dfa-91a6-d82a5fb8de12">LocalFree</a> (on *<i>pbPropertyValue</i>) to free the allocated memory. If no value is required, pass <b>NULL</b> for this parameter.


### -param pcbPropertyValueSize [out]

Pointer to the size, in bytes, of the value returned. If no size is required, pass <b>NULL</b> for this parameter.


## -returns



If the operations succeeds, the function returns <b>ERROR_SUCCESS</b>.

If the operation fails, 
the function returns a <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">system error code</a>. The following are possible error codes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_DATA</b></dt>
</dl>
</td>
<td width="60%">
The property list is incorrectly formatted.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
The function could not allocate a buffer in which to return the property value.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_FILE_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The specified property could not be located in the property list.

</td>
</tr>
</table>
 




## -remarks



If  <b>ResUtilFindMultiSzProperty</b> is successful, *<i>pbPropertyValue</i> points to a copy of the data stored in <i>pPropertyList</i>. Be sure to call <a href="https://msdn.microsoft.com/a0393983-cb43-4dfa-91a6-d82a5fb8de12">LocalFree</a> on *<i>pbPropertyValue</i> to prevent memory leaks.




## -see-also




<a href="https://msdn.microsoft.com/3be864ae-dc02-47e7-aa86-a6c14be13091">ResUtilFindBinaryProperty</a>



<a href="https://msdn.microsoft.com/884e922f-5cc6-4e46-b2f6-2436e7fc634e">ResUtilFindDwordProperty</a>



<a href="https://msdn.microsoft.com/44fb21bd-6cc2-4b1b-ae8f-c977fa336747">ResUtilFindExpandSzProperty</a>



<a href="https://msdn.microsoft.com/7a639932-6dd5-41ef-a126-c2d5001a436f">ResUtilFindExpandedSzProperty</a>



<a href="https://msdn.microsoft.com/6f75be85-37ef-4e2b-a588-bc1238cd8760">ResUtilFindLongProperty</a>



<a href="https://msdn.microsoft.com/b7fb6c7e-5a13-4838-98f4-45931e9e96d0">ResUtilFindSzProperty</a>
 

 
