---
UID: NS:d3d11shader._D3D11_FUNCTION_DESC
title: D3D11_FUNCTION_DESC
author: windows-sdk-content
description: Describes a function.
old-location: direct3d11\d3d11_function_desc.htm
tech.root: direct3d11
ms.assetid: 1C163EE4-DA67-4341-ACA3-13ACCDD1E952
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: D3D11_FUNCTION_DESC, D3D11_FUNCTION_DESC structure [Direct3D 11], d3d11shader/D3D11_FUNCTION_DESC, direct3d11.d3d11_function_desc
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: d3d11shader.h
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
 - D3D11Shader.h
api_name:
 - D3D11_FUNCTION_DESC
product: Windows
targetos: Windows
req.typenames: D3D11_FUNCTION_DESC
req.redist: 
---

# D3D11_FUNCTION_DESC structure


## -description


Describes a function.


## -struct-fields




### -field Version

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The shader version.


### -field Creator

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCSTR</a></b>

The name of the originator of the function.


### -field Flags

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

A combination of <a href="https://msdn.microsoft.com/039627DD-D6A4-4EA3-8E91-D2A20770E6FF">D3DCOMPILE Constants</a> that are combined by using a bitwise OR operation. The resulting value specifies shader compilation and parsing.


### -field ConstantBuffers

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of constant buffers for the function.


### -field BoundResources

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of bound resources for the function.


### -field InstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of emitted instructions for the function.


### -field TempRegisterCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of temporary registers used by the function.


### -field TempArrayCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of temporary arrays used by the function.


### -field DefCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of constant defines for the function.


### -field DclCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of declarations (input + output) for the function.


### -field TextureNormalInstructions

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of non-categorized texture instructions for the function.


### -field TextureLoadInstructions

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of texture load instructions for the function.


### -field TextureCompInstructions

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of texture comparison instructions for the function.


### -field TextureBiasInstructions

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of texture bias instructions for the function.


### -field TextureGradientInstructions

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of texture gradient instructions for the function.


### -field FloatInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of floating point arithmetic instructions used by the function.


### -field IntInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of signed integer arithmetic instructions used by the function.


### -field UintInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of unsigned integer arithmetic instructions used by the function.


### -field StaticFlowControlCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of static flow control instructions used by the function.


### -field DynamicFlowControlCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of dynamic flow control instructions used by the function.


### -field MacroInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of macro instructions used by the function.


### -field ArrayInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of array instructions used by the function.


### -field MovInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of mov instructions used by the function.


### -field MovcInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of movc instructions used by the function.


### -field ConversionInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of type conversion instructions used by the function.


### -field BitwiseInstructionCount

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of bitwise arithmetic instructions used by the function.


### -field MinFeatureLevel

Type: <b><a href="https://msdn.microsoft.com/afbc1a02-1730-4502-af15-b668412d664c">D3D_FEATURE_LEVEL</a></b>

A <a href="https://msdn.microsoft.com/afbc1a02-1730-4502-af15-b668412d664c">D3D_FEATURE_LEVEL</a>-typed value that specifies the minimum Direct3D feature level target of the function byte code.


### -field RequiredFeatureFlags

Type: <b>UINT64</b>

A value that contains a combination of one or more shader requirements flags; each flag specifies a requirement of the shader. A default value of 0 means there are no requirements. For a list of values, see <a href="https://msdn.microsoft.com/BC70E68A-8909-42F9-9AEE-017BA682D635">ID3D11ShaderReflection::GetRequiresFlags</a>. 


### -field Name

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPCSTR</a></b>

The name of the function.


### -field FunctionParameterCount

Type: <b>INT</b>

The number of logical parameters in the function signature, not including the return value.


### -field HasReturn

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

Indicates whether the function returns a value. <b>TRUE</b> indicates it returns a value; otherwise, <b>FALSE</b> (it is a subroutine).


### -field Has10Level9VertexShader

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

Indicates whether there is a Direct3D 10Level9 vertex shader blob. <b>TRUE</b> indicates there is a 10Level9 vertex shader blob; otherwise, <b>FALSE</b>.


### -field Has10Level9PixelShader

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">BOOL</a></b>

Indicates whether there is a Direct3D 10Level9 pixel shader blob. <b>TRUE</b> indicates there is a 10Level9 pixel shader blob; otherwise, <b>FALSE</b>.


## -see-also




<a href="https://msdn.microsoft.com/CD4A0602-BF89-4B17-99E3-35293FB0B66C">ID3D11FunctionReflection::GetDesc</a>



<a href="https://msdn.microsoft.com/3b8ece5c-5065-4711-b12c-06cf7ea0e1ba">Shader Structures</a>
 

 
