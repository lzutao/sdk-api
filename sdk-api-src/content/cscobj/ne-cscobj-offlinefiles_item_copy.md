---
UID: NE:cscobj.tagOFFLINEFILES_ITEM_COPY
title: OFFLINEFILES_ITEM_COPY
author: windows-sdk-content
description: Specifies whether the local, remote, or original copy of an item is being queried.
old-location: of\offlinefiles_item_copy.htm
tech.root: offlinefiles
ms.assetid: b956f186-962b-457e-9c03-ffd1a7f937ca
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: OFFLINEFILES_ITEM_COPY, OFFLINEFILES_ITEM_COPY enumeration [Offline Files], OFFLINEFILES_ITEM_COPY_LOCAL, OFFLINEFILES_ITEM_COPY_ORIGINAL, OFFLINEFILES_ITEM_COPY_REMOTE, cscobj/OFFLINEFILES_ITEM_COPY, cscobj/OFFLINEFILES_ITEM_COPY_LOCAL, cscobj/OFFLINEFILES_ITEM_COPY_ORIGINAL, cscobj/OFFLINEFILES_ITEM_COPY_REMOTE, of.offlinefiles_item_copy
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
 - CscObj.h
api_name:
 - OFFLINEFILES_ITEM_COPY
product: Windows
targetos: Windows
req.typenames: OFFLINEFILES_ITEM_COPY
req.redist: 
---

# OFFLINEFILES_ITEM_COPY enumeration


## -description


Specifies whether the local, remote, or original copy of an item is being queried.


## -enum-fields




### -field OFFLINEFILES_ITEM_COPY_LOCAL

Retrieve the attributes, time values, or size  of the local copy of the item.  If the item is currently offline, this may be different than the attributes associated with the original copy.


### -field OFFLINEFILES_ITEM_COPY_REMOTE

This enumeration value is reserved for future use.


### -field OFFLINEFILES_ITEM_COPY_ORIGINAL

Retrieve the attributes, time values, or size of the original copy of the item.  The original copy represents the state of the item following the last successful sync of that item, which is the most recent time when the server copy and local copy were identical.


## -see-also




<a href="https://msdn.microsoft.com/5bf8a834-cd5e-46b9-9b7d-b5cc6fb9fe10">IOfflineFilesFileSysInfo::GetAttributes</a>



<a href="https://msdn.microsoft.com/a24b7126-ee9a-40f8-9fcd-8696e756a6b9">IOfflineFilesFileSysInfo::GetFileSize</a>



<a href="https://msdn.microsoft.com/120b3f7c-6a92-4a03-8676-1ad4e4dc96b3">IOfflineFilesFileSysInfo::GetTimes</a>
 

 
