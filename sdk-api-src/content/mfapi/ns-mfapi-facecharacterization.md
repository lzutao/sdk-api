---
UID: NS:mfapi.tagFaceCharacterization
title: FaceCharacterization
author: windows-sdk-content
description: The FaceCharacterization structure describes the blob format for the MF_CAPTURE_METADATA_FACEROICHARACTERIZATIONS attribute.
old-location: stream\facecharacterization.htm
tech.root: stream
ms.assetid: 8A8F6E06-DA09-4595-BF42-8B905453CCCA
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: FaceCharacterization, FaceCharacterization structure [Streaming Media Devices], mfapi/FaceCharacterization, stream.facecharacterization
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: mfapi.h
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
 - mfapi.h
api_name:
 - FaceCharacterization
product: Windows
targetos: Windows
req.typenames: FaceCharacterization
req.redist: 
---

# FaceCharacterization structure


## -description


The <b>FaceCharacterization</b> structure describes the blob format for the <b>MF_CAPTURE_METADATA_FACEROICHARACTERIZATIONS</b> attribute.


## -struct-fields




### -field BlinkScoreLeft

0 indicates no blink for the left eye, 100 indicates definite blink for the left eye (0 - 100).


### -field BlinkScoreRight

0 indicates no blink for the right eye, 100 indicates definite blink for the right eye (0 - 100).


### -field FacialExpression

A  defined facial expression value.


### -field FacialExpressionScore

0 indicates no such facial expression as identified, 100 indicates definite such facial expression as defined (0 - 100).


## -remarks



The <b>MF_CAPTURE_METADATA_FACEROICHARACTERIZATIONS</b> attribute contains the blink and facial expression state for the face ROIs identified in <b>MF_CAPTURE_METADATA_FACEROIS</b>.  For a  device that does not support blink or facial expression detection, this attribute should be omitted.

The facial expressions that can be detected are defined as follows:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>#define MF_METADATAFACIALEXPRESSION_SMILE             0x00000001</pre>
</td>
</tr>
</table></span></div>
The <a href="https://msdn.microsoft.com/F3BDB935-A8CB-41BA-B912-0B9264FE0B09">FaceCharacterizationBlobHeader</a> and <b>FaceCharacterization</b> structures only describe the blob format for the <b>MF_CAPTURE_METADATA_FACEROICHARACTERIZATIONS</b> attribute.  The metadata item structure for the face characterizations (<a href="https://msdn.microsoft.com/B4AC04D7-9F98-41F1-A38D-927F3F3A7699">KSCAMERA_METADATA_ITEMHEADER</a> + face characterizations metadata payload) is up to driver and must be 8-byte aligned. 


