---
UID: NF:wbemglue.CWbemProviderGlue.FrameworkLogoffDLL(LPCWSTR,PLONG)
title: CWbemProviderGlue::FrameworkLogoffDLL(LPCWSTR,PLONG)
author: windows-sdk-content
description: The FrameworkLogoffDLL method is called by DllCanUnloadNow to determine whether the provider server is not in use and can be unloaded.
old-location: wmi\cwbemproviderglue_frameworklogoffdll.htm
tech.root: WmiSdk
ms.assetid: 5157d823-d3a1-46d2-8ae8-07e904001a14
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "?FrameworkLogoffDLL@CWbemProviderGlue@@SAHPEBG@Z, ?FrameworkLogoffDLL@CWbemProviderGlue@@SGHPBG@Z, CWbemProviderGlue interface [Windows Management Instrumentation],FrameworkLogoffDLL method, CWbemProviderGlue.FrameworkLogoffDLL, CWbemProviderGlue.FrameworkLogoffDLL(LPCWSTR,PLONG), CWbemProviderGlue::FrameworkLogoffDLL, CWbemProviderGlue::FrameworkLogoffDLL(LPCWSTR,PLONG), FrameworkLogoffDLL, FrameworkLogoffDLL method [Windows Management Instrumentation], FrameworkLogoffDLL method [Windows Management Instrumentation],CWbemProviderGlue interface, _hmm_cwbemproviderglue_frameworklogoffdll, wbemglue/CWbemProviderGlue::FrameworkLogoffDLL, wmi.cwbemproviderglue_frameworklogoffdll"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wbemglue.h
req.include-header: FwCommon.h
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
req.lib: FrameDyn.lib
req.dll: FrameDynOS.dll; FrameDyn.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - FrameDynOS.dll
 - FrameDyn.dll
api_name:
 - CWbemProviderGlue.FrameworkLogoffDLL
 - ?FrameworkLogoffDLL@CWbemProviderGlue@@SAHPEBG@Z
 - ?FrameworkLogoffDLL@CWbemProviderGlue@@SGHPBG@Z
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# CWbemProviderGlue::FrameworkLogoffDLL(LPCWSTR,PLONG)


## -description


<p class="CCE_Message">[The <a href="https://msdn.microsoft.com/493027c2-e54d-4fad-9e33-98d1ceab8860">CWbemProviderGlue</a> class 
    is part of the WMI Provider Framework which is now considered in final state, and no further development, 
    enhancements, or updates will be available for non-security related issues affecting these libraries. The 
    <a href="https://msdn.microsoft.com/7F311E1B-5CE6-488D-9411-DE1822D95C3B">MI APIs</a> should be used for all new 
    development.]

The <b>FrameworkLogoffDLL</b> method is called by <b>DllCanUnloadNow</b> to determine whether the provider server is not in use and can be unloaded.


## -parameters




### -param name

Name of the server that is unloaded.


### -param plRefCount

TBD




## -returns



The method returns <b>TRUE</b> if the server is not in use and can be unloaded and <b>FALSE</b> if the server is still in use and cannot be unloaded.




## -remarks



For now,  <b>FrameworkLogoffDLL</b> returns <b>FALSE</b> until the refcount for <a href="https://msdn.microsoft.com/493027c2-e54d-4fad-9e33-98d1ceab8860">CWbemProviderGlue</a> is zero. This approach prevents unloading any client DLL while instances of <b>CWbemProviderGlue</b> still exist.


