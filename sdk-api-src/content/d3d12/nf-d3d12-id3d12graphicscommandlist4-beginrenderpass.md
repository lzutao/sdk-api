---
UID: NF:d3d12.ID3D12GraphicsCommandList4.BeginRenderPass
title: ID3D12GraphicsCommandList4::BeginRenderPass
author: windows-sdk-content
description: Marks the beginning of a render pass by binding a set of output resources for the duration of the render pass. These bindings are to one or more render target views (RTVs), and/or to a depth stencil view (DSV).
old-location: direct3d12\id3d12graphicscommandlist4_beginrenderpass.htm
tech.root: direct3d12
ms.assetid: 6A7CF754-F2E6-48D4-8A4D-CE64B31267F7
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: BeginRenderPass, BeginRenderPass method, BeginRenderPass method,ID3D12GraphicsCommandList4 interface, ID3D12GraphicsCommandList4 interface,BeginRenderPass method, ID3D12GraphicsCommandList4.BeginRenderPass, ID3D12GraphicsCommandList4::BeginRenderPass, d3d12/ID3D12GraphicsCommandList4::BeginRenderPass, direct3d12.id3d12graphicscommandlist4_beginrenderpass
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d12.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1809 [desktop apps only]
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
req.lib: D3D12.lib
req.dll: D3D12.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D12.dll
api_name:
 - ID3D12GraphicsCommandList4.BeginRenderPass
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D12GraphicsCommandList4::BeginRenderPass


## -description


Marks the beginning of a render pass by binding a set of output resources for the duration of the render pass. These bindings are to one or more render target views (RTVs), and/or to a depth stencil view (DSV).


## -parameters




### -param NumRenderTargets

A <b>UINT</b>. The number of render targets being bound.


### -param pRenderTargets

A pointer to a constant <a href="https://msdn.microsoft.com/C319081F-290E-4031-AE0C-F97D82ED4178">D3D12_RENDER_PASS_RENDER_TARGET_DESC</a>, which describes bindings (fixed for the duration of the render pass) to one or more render target views (RTVs), as well as their beginning and ending access characteristics.


### -param pDepthStencil

A pointer to a constant <a href="https://msdn.microsoft.com/1C67A6D0-F912-471F-A38C-E3C6A74303EF">D3D12_RENDER_PASS_DEPTH_STENCIL_DESC</a>, which describes a binding (fixed for the duration of the render pass) to a depth stencil view (DSV), as well as its beginning and ending access characteristics.


### -param Flags

A <a href="https://msdn.microsoft.com/4F1D13BD-60BC-4CE7-9671-42886989FE31">D3D12_RENDER_PASS_FLAGS</a>. The nature/requirements of the render pass; for example, whether it is a suspending or a resuming render pass, or whether it wants to write to unordered access view(s).


## -returns



This method does not return a value.




## -see-also




<a href="https://msdn.microsoft.com/6CFF2A67-F2F0-41F8-8BEC-D52003DE2767">EndRenderPass</a>



<a href="https://msdn.microsoft.com/en-us/library/Mt847460(v=VS.85).aspx">ID3D12GraphicsCommandList4</a>
 

 
