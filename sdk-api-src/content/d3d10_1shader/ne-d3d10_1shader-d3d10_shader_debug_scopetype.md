---
UID: NE:d3d10_1shader._D3D10_SHADER_DEBUG_SCOPETYPE
title: D3D10_SHADER_DEBUG_SCOPETYPE
author: windows-sdk-content
description: Scope types.
old-location: direct3d10\d3d10_shader_debug_scopetype.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\d3d10_shader_debug_scopetype.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D10_SHADER_DEBUG_SCOPETYPE, D3D10_SHADER_DEBUG_SCOPETYPE enumeration [Direct3D 10], D3D10_SHADER_DEBUG_SCOPE_ANNOTATION, D3D10_SHADER_DEBUG_SCOPE_BLOCK, D3D10_SHADER_DEBUG_SCOPE_FORCE_DWORD, D3D10_SHADER_DEBUG_SCOPE_FORLOOP, D3D10_SHADER_DEBUG_SCOPE_FUNC_PARAMS, D3D10_SHADER_DEBUG_SCOPE_GLOBAL, D3D10_SHADER_DEBUG_SCOPE_NAMESPACE, D3D10_SHADER_DEBUG_SCOPE_STATEBLOCK, D3D10_SHADER_DEBUG_SCOPE_STRUCT, a42aff03-01b4-0000-857a-579862c3b15e, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPETYPE, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_ANNOTATION, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_BLOCK, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_FORCE_DWORD, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_FORLOOP, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_FUNC_PARAMS, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_GLOBAL, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_NAMESPACE, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_STATEBLOCK, d3d10_1shader/D3D10_SHADER_DEBUG_SCOPE_STRUCT, direct3d10.d3d10_shader_debug_scopetype
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: d3d10_1shader.h
req.include-header: D3D10Shader.h
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
 - d3d10_1shader.h
api_name:
 - D3D10_SHADER_DEBUG_SCOPETYPE
product: Windows
targetos: Windows
req.typenames: D3D10_SHADER_DEBUG_SCOPETYPE
req.redist: 
---

# D3D10_SHADER_DEBUG_SCOPETYPE enumeration


## -description


Scope types.


## -enum-fields




### -field D3D10_SHADER_DEBUG_SCOPE_GLOBAL

Global scope.


### -field D3D10_SHADER_DEBUG_SCOPE_BLOCK

Block scope.


### -field D3D10_SHADER_DEBUG_SCOPE_FORLOOP

For loop scope.


### -field D3D10_SHADER_DEBUG_SCOPE_STRUCT

Structure scope.


### -field D3D10_SHADER_DEBUG_SCOPE_FUNC_PARAMS

Function parameter scope.


### -field D3D10_SHADER_DEBUG_SCOPE_STATEBLOCK

State block scope.


### -field D3D10_SHADER_DEBUG_SCOPE_NAMESPACE

Name space scope.


### -field D3D10_SHADER_DEBUG_SCOPE_ANNOTATION

Annotation scope.


### -field D3D10_SHADER_DEBUG_SCOPE_FORCE_DWORD

Forces this enumeration to compile to 32 bits in size. Without this value, some compilers would allow this enumeration to compile to a size other than 32 bits. This value is not used.


## -remarks



The <b>D3D10_SHADER_DEBUG_SCOPETYPE</b> enumeration is used to specify scope type in the <a href="https://msdn.microsoft.com/ccee4d4b-86e2-441c-abc1-2aba1163f149">D3D10_SHADER_DEBUG_SCOPE_INFO</a> structure.




## -see-also




<a href="https://msdn.microsoft.com/8d2b758b-cc2a-43ad-bf26-51674d4b5129">Shader Enumerations</a>
 

 
