---
UID: NS:commctrl.tagNMREBARSPLITTER
title: NMREBARSPLITTER
author: windows-sdk-content
description: Contains information used to handle an RBN_SPLITTERDRAG notification code.
old-location: controls\NMREBARSPLITTER.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\rebar\structures\nmrebarsplitter.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPNMREBARSPLITTER, LPNMREBARSPLITTER, LPNMREBARSPLITTER structure pointer [Windows Controls], NMREBARSPLITTER, NMREBARSPLITTER structure [Windows Controls], _shell_NMREBARSPLITTER, _shell_NMREBARSPLITTER_cpp, commctrl/LPNMREBARSPLITTER, commctrl/NMREBARSPLITTER, controls.NMREBARSPLITTER, controls._shell_NMREBARSPLITTER"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
 - NMREBARSPLITTER
product: Windows
targetos: Windows
req.typenames: NMREBARSPLITTER, *LPNMREBARSPLITTER
req.redist: 
---

# NMREBARSPLITTER structure


## -description


Contains information used to handle an <a href="https://msdn.microsoft.com/en-us/library/Bb774427(v=VS.85).aspx">RBN_SPLITTERDRAG</a> notification code.


## -struct-fields




### -field hdr

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a></b>

An <a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a> structure that contains additional information about this notification. 


### -field rcSizing

Type: <b><a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a></b>

An <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that indicates the size the rebar will be after the drag operation completes.
