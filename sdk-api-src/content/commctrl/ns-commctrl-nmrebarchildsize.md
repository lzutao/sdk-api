---
UID: NS:commctrl.tagNMREBARCHILDSIZE
title: NMREBARCHILDSIZE
author: windows-sdk-content
description: Contains information used in handling the RBN_CHILDSIZE notification code.
old-location: controls\NMREBARCHILDSIZE.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\rebar\structures\nmrebarchildsize.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPNMREBARCHILDSIZE, LPNMREBARCHILDSIZE, LPNMREBARCHILDSIZE structure pointer [Windows Controls], NMREBARCHILDSIZE, NMREBARCHILDSIZE structure [Windows Controls], _win32_NMREBARCHILDSIZE, _win32_NMREBARCHILDSIZE_cpp, commctrl/LPNMREBARCHILDSIZE, commctrl/NMREBARCHILDSIZE, controls.NMREBARCHILDSIZE, controls._win32_NMREBARCHILDSIZE"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - Commctrl.h
api_name:
 - NMREBARCHILDSIZE
product: Windows
targetos: Windows
req.typenames: NMREBARCHILDSIZE, *LPNMREBARCHILDSIZE
req.redist: 
---

# NMREBARCHILDSIZE structure


## -description


Contains information used in handling the <a href="https://msdn.microsoft.com/en-us/library/Bb774411(v=VS.85).aspx">RBN_CHILDSIZE</a> notification code. 


## -struct-fields




### -field hdr

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a> structure that contains additional information about the notification. 


### -field uBand

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Zero-based index of the band affected by the notification. This will be -1 if no band is affected. 


### -field wID

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

Application-defined identifier of the band. 


### -field rcChild

Type: <b><a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a></b>


<a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that contains the new size of the child window. This member can be changed during the notification to modify the child window's position and size. 


### -field rcBand

Type: <b><a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a></b>


<a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that contains the new size of the band. 
