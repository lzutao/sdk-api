---
UID: NF:mmiscapi.DrvDefDriverProc
title: DrvDefDriverProc function
author: windows-sdk-content
description: Provides default processing for any messages not processed by an installable driver. This function is intended to be used only within the DriverProc function of an installable driver.
old-location: multimedia\defdriverproc.htm
tech.root: Multimedia
ms.assetid: 8401925b-d286-41bd-b57e-838b2f5b250d
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DefDriverProc, DefDriverProc function [Windows Multimedia], DrvDefDriverProc, _win32_DefDriverProc, mmsystem/DefDriverProc, multimedia.defdriverproc
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: mmiscapi.h
req.include-header: Mmiscapi.h, Windows.h
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
req.lib: Winmm.lib
req.dll: Winmm.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Winmm.dll
 - API-MS-Win-mm-misc-l1-1-0.dll
 - winmmbase.dll
 - API-MS-Win-mm-misc-l1-1-1.dll
api_name:
 - DefDriverProc
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# DrvDefDriverProc function


## -description



Provides default processing for any messages not processed by an installable driver. This function is intended to be used only within the <a href="https://msdn.microsoft.com/d9a5535f-6b80-40cc-a20b-b7a342414d7f">DriverProc</a> function of an installable driver.




## -parameters




### -param dwDriverIdentifier

Identifier of the installable driver.


### -param hdrvr

Handle of the installable driver instance.


### -param uMsg

Driver message value.


### -param lParam1

32-bit message-dependent information.


### -param lParam2

32-bit message-dependent information.


## -returns



Returns nonzero if successful or zero otherwise.


