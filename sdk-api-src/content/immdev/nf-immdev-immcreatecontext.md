---
UID: NF:immdev.ImmCreateContext
title: ImmCreateContext function
author: windows-sdk-content
description: Creates a new input context, allocating memory for the context and initializing it. An application calls this function to prepare its own input context.
old-location: intl\immcreatecontext.htm
tech.root: Intl
ms.assetid: 2207927a-0edb-4d3a-a1b7-75b94d1616d5
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ImmCreateContext, ImmCreateContext function [Internationalization for Windows Applications], _win32_ImmCreateContext, imm/ImmCreateContext, intl.immcreatecontext
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
 - imm32.dll
api_name:
 - ImmCreateContext
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ImmCreateContext function


## -description


Creates a new input context, allocating memory for the context and initializing it. An application calls this function to prepare its own input context.


## -parameters






## -returns



Returns the handle to the new input context if successful, or <b>NULL</b> otherwise.




## -see-also




<a href="https://msdn.microsoft.com/3e23e004-514a-4021-bd20-5ac55547258f">Input Method Manager</a>



<a href="https://msdn.microsoft.com/833c07eb-0ecf-41e2-9e01-8d83e51ffcef">Input Method Manager Functions</a>
 

 
