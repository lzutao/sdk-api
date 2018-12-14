---
UID: NS:mi._MI_ConstReal32Field
title: MI_ConstReal32Field
author: windows-sdk-content
description: Represents a property inside an MI_Instance structure.
old-location: wmi_v2\mi_constreal32field.htm
tech.root: wmi_v2
ms.assetid: 3bf3a9fb-215c-44c2-9aa6-40c3af82c949
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MI_ConstReal32Field, MI_ConstReal32Field structure [Windows Management Infrastructure (MI)], MI_FLAG_ADOPT, MI_FLAG_BORROW, MI_FLAG_NOT_MODIFIED, MI_FLAG_NULL, mi/MI_ConstReal32Field, wmi._mi_constreal32field, wmi_v2.mi_constreal32field
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: mi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Mi.h
api_name:
 - MI_ConstReal32Field
product: Windows
targetos: Windows
req.typenames: MI_ConstReal32Field
req.redist: Windows Management Framework 3.0 on Windows Server 2008 R2 with SP1, Windows 7 with SP1, and Windows Server 2008 with SP2
---

# MI_ConstReal32Field structure


## -description


Represents a property inside an <a href="https://msdn.microsoft.com/3dce1817-7995-49e5-8cc0-ee9496665e5c">MI_Instance</a> structure.


## -struct-fields




### -field value

A field of type <b>MI_Real32</b>.


### -field exists

Indicates whether the field is non-null. Can be set to <b>MI_TRUE</b> or <b>MI_FALSE</b>.


### -field flags

Bit flags indicating memory management policy.



#### MI_FLAG_NOT_MODIFIED ((1 << 25))

Indicates that the property is not modified.



#### MI_FLAG_NULL ((1 << 29))

Element value is <b>Null</b>.



#### MI_FLAG_BORROW ((1 << 30))

Used while adding and setting properties on an <b>MI_Instance</b> to indicate that the instance will not copy the value. The value must stay valid until the instance is deleted.



#### MI_FLAG_ADOPT ((1 << 31))

Used while adding and setting properties on an <b>MI_Instance</b> to indicate that the instance will adopt the pointer and will be responsible for deleting it.
