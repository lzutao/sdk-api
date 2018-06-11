---
UID: NE:vdssys._DELETE_SNAPSHOT_VHDSET_FLAG
title: "_DELETE_SNAPSHOT_VHDSET_FLAG"
author: windows-sdk-content
description: Contains flags affecting the behavior of the DeleteSnapshotVhdSet function.
old-location: vhd\delete_snapshot_vhdset_flag.htm
old-project: VStor
ms.assetid: 42B56389-8ECE-4127-A641-7F0A0A1E7D2D
ms.author: windowssdkdev
ms.date: 05/29/2018
ms.keywords: "*PDELETE_SNAPSHOT_VHDSET_FLAG, DELETE_SNAPSHOT_VHDSET_FLAG, DELETE_SNAPSHOT_VHDSET_FLAG enumeration [VHD], DELETE_SNAPSHOT_VHDSET_FLAG_NONE, DELETE_SNAPSHOT_VHDSET_FLAG_PERSIST_RCT, PDELETE_SNAPSHOT_VHDSET_FLAG, PDELETE_SNAPSHOT_VHDSET_FLAG enumeration pointer [VHD], _DELETE_SNAPSHOT_VHDSET_FLAG, vdssys/DELETE_SNAPSHOT_VHDSET_FLAG, vdssys/DELETE_SNAPSHOT_VHDSET_FLAG_NONE, vdssys/DELETE_SNAPSHOT_VHDSET_FLAG_PERSIST_RCT, vdssys/PDELETE_SNAPSHOT_VHDSET_FLAG, vhd.delete_snapshot_vhdset_flag, virtdisk/DELETE_SNAPSHOT_VHDSET_FLAG, virtdisk/DELETE_SNAPSHOT_VHDSET_FLAG_NONE, virtdisk/DELETE_SNAPSHOT_VHDSET_FLAG_PERSIST_RCT, virtdisk/PDELETE_SNAPSHOT_VHDSET_FLAG"
ms.prod: windows
ms.technology: windows-sdk
ms.topic: enum
req.header: vdssys.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server 2016 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
tech.root: 
req.typenames: DELETE_SNAPSHOT_VHDSET_FLAG, *PDELETE_SNAPSHOT_VHDSET_FLAG
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - VirtDisk.h
 - vdssys.h
api_name:
 - DELETE_SNAPSHOT_VHDSET_FLAG
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Windows UI
---

# _DELETE_SNAPSHOT_VHDSET_FLAG enumeration


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

Contains flags affecting the behavior of the <a href="https://msdn.microsoft.com/F6A65E00-857A-44CF-A827-747518564DAB">DeleteSnapshotVhdSet</a> function.


## -enum-fields




### -field DELETE_SNAPSHOT_VHDSET_FLAG_NONE

No flag specified.


### -field DELETE_SNAPSHOT_VHDSET_FLAG_PERSIST_RCT

A reference point should be persisted in the VHD Set after the snapshot is deleted.
