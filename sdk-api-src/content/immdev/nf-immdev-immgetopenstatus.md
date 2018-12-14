---
UID: NF:immdev.ImmGetOpenStatus
title: ImmGetOpenStatus function
author: windows-sdk-content
description: Determines whether the IME is open or closed.
old-location: intl\immgetopenstatus.htm
tech.root: Intl
ms.assetid: 8011bb84-9bda-49b7-8f44-76af4388ce21
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ImmGetOpenStatus, ImmGetOpenStatus function [Internationalization for Windows Applications], _win32_ImmGetOpenStatus, imm/ImmGetOpenStatus, intl.immgetopenstatus
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: immdev.h
req.include-header: Immdev.h, Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only],East Asian language support installed.
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
req.lib: Imm32.lib
req.dll: Imm32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Imm32.dll
 - Ext-MS-Win-imm-l1-1-0.dll
 - ext-ms-win-imm-l1-1-1.dll
api_name:
 - ImmGetOpenStatus
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ImmGetOpenStatus function


## -description


Determines whether the IME is open or closed.


## -parameters




### -param HIMC [in]

Handle to the input context.


## -returns



Returns a nonzero value if the IME is open, or 0 otherwise.




## -see-also




<a href="https://msdn.microsoft.com/3e23e004-514a-4021-bd20-5ac55547258f">Input Method Manager</a>



<a href="https://msdn.microsoft.com/833c07eb-0ecf-41e2-9e01-8d83e51ffcef">Input Method Manager Functions</a>
 

 
