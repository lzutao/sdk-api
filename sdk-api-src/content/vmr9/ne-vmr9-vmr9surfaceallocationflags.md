---
UID: NE:vmr9.__MIDL___MIDL_itf_vmr9_0000_0001_0001
title: VMR9SurfaceAllocationFlags
author: windows-sdk-content
description: The VMR9SurfaceAllocationFlags enumeration type is used with the IVMRSurfaceAllocator9::InitializeDevice method to specify surface creation parameters (VMR-9 only).
old-location: dshow\vmr9surfaceallocationflags.htm
tech.root: DirectShow
ms.assetid: 880e6c78-177f-49d0-a526-5f036c715f9e
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: VMR9AllocFlag_3DRenderTarget, VMR9AllocFlag_DXVATarget, VMR9AllocFlag_OffscreenSurface, VMR9AllocFlag_RGBDynamicSwitch, VMR9AllocFlag_TextureSurface, VMR9AllocFlag_UsageMask, VMR9AllocFlag_UsageReserved, VMR9SurfaceAllocationFlags, VMR9SurfaceAllocationFlags , VMR9SurfaceAllocationFlags enumeration [DirectShow], VMR9SurfaceAllocationFlagsEnumeration, dshow.vmr9surfaceallocationflags, vmr9/VMR9AllocFlag_3DRenderTarget, vmr9/VMR9AllocFlag_DXVATarget, vmr9/VMR9AllocFlag_OffscreenSurface, vmr9/VMR9AllocFlag_RGBDynamicSwitch, vmr9/VMR9AllocFlag_TextureSurface, vmr9/VMR9AllocFlag_UsageMask, vmr9/VMR9AllocFlag_UsageReserved, vmr9/VMR9SurfaceAllocationFlags
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: vmr9.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
 - Vmr9.h
api_name:
 - VMR9SurfaceAllocationFlags
product: Windows
targetos: Windows
req.typenames: VMR9SurfaceAllocationFlags
req.redist: 
---

# VMR9SurfaceAllocationFlags enumeration


## -description



The <b>VMR9SurfaceAllocationFlags</b> enumeration type is used with the <a href="https://msdn.microsoft.com/44c22dc0-98a9-4a6e-a488-1d70dfff6acd">IVMRSurfaceAllocator9::InitializeDevice</a> method to specify surface creation parameters (VMR-9 only).




## -enum-fields




### -field VMR9AllocFlag_3DRenderTarget

Indicates that the surface is a Direct3D render target.


### -field VMR9AllocFlag_DXVATarget

Indicates that the render target supports DXVA.


### -field VMR9AllocFlag_TextureSurface

Indicates that the target is a Direct3D texture surface.


### -field VMR9AllocFlag_OffscreenSurface

Indicates an offscreen surface.


### -field VMR9AllocFlag_RGBDynamicSwitch

In YUV mixing mode, indicates that the mixer can accept RGB formats in addition to the specified YUV format. The allocator-presenter can switch between the formats dynamically. This flag is only valid in YUV mixing mode.


### -field VMR9AllocFlag_UsageReserved

Reserved for future use.


### -field VMR9AllocFlag_UsageMask

Bitwise <b>OR</b> of all flags; not used by applications


## -remarks



The VMR9AllocFlag_TextureSurface flag can be combined with the VMR9AllocFlag_DXVATarget and VMR9AllocFlag_3DRenderTarget flags.




## -see-also




<a href="https://msdn.microsoft.com/74467006-b077-49c0-8573-f939ac3d3444">DirectShow Enumerated Types</a>
 

 
