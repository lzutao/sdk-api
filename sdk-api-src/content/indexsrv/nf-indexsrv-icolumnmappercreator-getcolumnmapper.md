---
UID: NF:indexsrv.IColumnMapperCreator.GetColumnMapper
title: IColumnMapperCreator::GetColumnMapper
author: windows-sdk-content
description: Retrieves a column mapper object.
old-location: search\icolumnmappercreator_getcolumnmapper.htm
tech.root: search
ms.assetid: DFFB27B0-EB82-41A4-A7EE-82495023DD2D
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetColumnMapper, GetColumnMapper method [search], GetColumnMapper method [search],IColumnMapperCreator interface, IColumnMapperCreator interface [search],GetColumnMapper method, IColumnMapperCreator.GetColumnMapper, IColumnMapperCreator::GetColumnMapper, indexsrv/IColumnMapperCreator::GetColumnMapper, search.icolumnmappercreator_getcolumnmapper
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: indexsrv.h
req.include-header: 
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
 - COM
api_location:
 - indexsrv.h
api_name:
 - IColumnMapperCreator.GetColumnMapper
product: Windows
targetos: Windows
req.typenames: 
req.redist: Windows NT 4.0 Option Pack
---

# IColumnMapperCreator::GetColumnMapper


## -description


Retrieves a column mapper object.


## -parameters




### -param wcsMachineName [in]

Machine on which the catalog exists.


### -param wcsCatalogName [in]

Catalog for which column mapper is requested.


### -param ppColumnMapper [out]

Stores the outgoing column mapper pointer.


## -returns



If this method succeeds, it returns <b>S_OK</b>. Otherwise, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/3598C736-5736-4B08-83B7-E80BA69FCBAB">IColumnMapperCreator</a>
 

 
