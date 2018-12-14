---
UID: NS:rpcdce._UUID_VECTOR
title: UUID_VECTOR
author: windows-sdk-content
description: The UUID_VECTOR structure contains a list of UUIDs.
old-location: rpc\uuid_vector.htm
tech.root: rpc
ms.assetid: 6fc7216b-023b-4aca-a572-35cc22202522
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: UUID_VECTOR, UUID_VECTOR structure [RPC], _rpc_uuid_vector, rpc.uuid_vector, rpcdce/UUID_VECTOR
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: rpcdce.h
req.include-header: Rpc.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - Rpcdce.h
api_name:
 - UUID_VECTOR
product: Windows
targetos: Windows
req.typenames: UUID_VECTOR
req.redist: 
---

# UUID_VECTOR structure


## -description


The 
<b>UUID_VECTOR</b> structure contains a list of <a href="https://msdn.microsoft.com/14288352-43c3-4e4d-a3f1-e924a8261d2b">UUID</a>s.


## -struct-fields




### -field Count

Number of <a href="https://msdn.microsoft.com/14288352-43c3-4e4d-a3f1-e924a8261d2b">UUID</a>s present in the array <b>Uuid</b>.
					


### -field Uuid

Array of pointers to <a href="https://msdn.microsoft.com/14288352-43c3-4e4d-a3f1-e924a8261d2b">UUID</a>s that contains <b>Count</b> elements.


## -remarks



The <a href="https://msdn.microsoft.com/14288352-43c3-4e4d-a3f1-e924a8261d2b">UUID</a> vector contains a count member containing the total number of <b>UUID</b>s in the vector, followed by an array of pointers to <b>UUID</b>s.

An application constructs a <a href="https://msdn.microsoft.com/14288352-43c3-4e4d-a3f1-e924a8261d2b">UUID</a> vector to contain object <b>UUID</b>s to be exported or unexported from the name service.




## -see-also




<a href="https://msdn.microsoft.com/35656cdd-b1ae-43d3-a5c7-92bdb7726d5b">RpcEpRegister</a>



<a href="https://msdn.microsoft.com/eaf132a8-0bc2-4201-945a-76b6c2eab559">RpcEpRegisterNoReplace</a>



<a href="https://msdn.microsoft.com/bb0485fc-0b25-4fc0-9a18-921a9de428ce">RpcEpUnregister</a>



<a href="https://msdn.microsoft.com/c89d04d7-f607-48cc-8cb6-b6aebab41671">RpcNsBindingExport</a>



<a href="https://msdn.microsoft.com/70662e7e-7a81-4953-9814-e29b46422c5b">RpcNsBindingUnexport</a>
 

 
