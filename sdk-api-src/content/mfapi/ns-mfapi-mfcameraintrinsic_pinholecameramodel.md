---
UID: NS:mfapi._MFCameraIntrinsic_PinholeCameraModel
title: MFCameraIntrinsic_PinholeCameraModel
author: windows-sdk-content
description: Represents a pinhole camera model.
old-location: mf\mfcameraintrinsic_pinholecameramodel.htm
tech.root: medfound
ms.assetid: 556DF8D8-F171-4055-86F1-F3258CC7D090
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: MFCameraIntrinsic_PinholeCameraModel, MFCameraIntrinsic_PinholeCameraModel structure [Media Foundation], PMFCameraIntrinsic_PinholeCameraModel, PMFCameraIntrinsic_PinholeCameraModel structure pointer [Media Foundation], mf.mfcameraintrinsic_pinholecameramodel, mfapi/MFCameraIntrinsic_PinholeCameraModel, mfapi/PMFCameraIntrinsic_PinholeCameraModel
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: mfapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - mfapi.h
api_name:
 - MFCameraIntrinsic_PinholeCameraModel
product: Windows
targetos: Windows
req.typenames: MFCameraIntrinsic_PinholeCameraModel
req.redist: 
---

# MFCameraIntrinsic_PinholeCameraModel structure


## -description


Represents a pinhole camera model. 


## -struct-fields




### -field FocalLength

The focal length of the camera.


### -field PrincipalPoint

The principal point of the camera.


## -remarks



For square pixels, the X and Y fields of the <b>FocalLength</b> should be the same.

The <b>PrincipalPoint</b> field is expressed in pixels, not in normalized coordinates. The  origin [0,0] is the bottom, left corner of the image.




## -see-also




<a href="https://msdn.microsoft.com/39fdd724-13ca-48ab-8a55-93529d1da3b4">Media Foundation Structures</a>
 

 
