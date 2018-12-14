---
UID: NS:commctrl.tagNMBCDROPDOWN
title: NMBCDROPDOWN
author: windows-sdk-content
description: Contains information about a BCN_DROPDOWN notification.
old-location: controls\NMBCDROPDOWN.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\buttons\buttonreference\buttonstructures\nmbcdropdown.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPNMBCDROPDOWN, LPNMBCDROPDOWN, LPNMBCDROPDOWN structure pointer [Windows Controls], NMBCDROPDOWN, NMBCDROPDOWN structure [Windows Controls], _shell_NMBCDROPDOWN, _shell_NMBCDROPDOWN_cpp, commctrl/LPNMBCDROPDOWN, commctrl/NMBCDROPDOWN, controls.NMBCDROPDOWN, controls._shell_NMBCDROPDOWN"
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
 - NMBCDROPDOWN
product: Windows
targetos: Windows
req.typenames: NMBCDROPDOWN, *LPNMBCDROPDOWN
req.redist: 
---

# NMBCDROPDOWN structure


## -description


Contains information about a <a href="https://msdn.microsoft.com/en-us/library/Bb775983(v=VS.85).aspx">BCN_DROPDOWN</a> notification.


## -struct-fields




### -field hdr

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a></b>

An <a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a> structure containing information about the notification.


### -field rcButton

Type: <b><a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a></b>

A <a href="https://msdn.microsoft.com/9439cb6c-f2f7-4c27-b1d7-8ddf16d81fe8">RECT</a> structure that contains the client area of the button.
