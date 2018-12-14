---
UID: NS:tapi.linemediacontroldigit_tag
title: LINEMEDIACONTROLDIGIT
author: windows-sdk-content
description: The LINEMEDIACONTROLDIGIT structure describes a media action to be executed when detecting a digit. It is used as an entry in an array. The lineSetMediaControl and TSPI_lineSetMediaControl functions use this structure.
old-location: tapi2\linemediacontroldigit_str.htm
tech.root: tapi
ms.assetid: d31cd365-d6a6-4595-8202-87113035d807
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPLINEMEDIACONTROLDIGIT, LINEMEDIACONTROLDIGIT, LINEMEDIACONTROLDIGIT structure [TAPI 2.2], LPLINEMEDIACONTROLDIGIT, LPLINEMEDIACONTROLDIGIT structure pointer [TAPI 2.2], _tapi2_linemediacontroldigit_str, tapi/LINEMEDIACONTROLDIGIT, tapi/LPLINEMEDIACONTROLDIGIT, tapi2.linemediacontroldigit_str"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: tapi.h
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
 - Tapi.h
api_name:
 - LINEMEDIACONTROLDIGIT
product: Windows
targetos: Windows
req.typenames: LINEMEDIACONTROLDIGIT, *LPLINEMEDIACONTROLDIGIT
req.redist: 
---

# LINEMEDIACONTROLDIGIT structure


## -description


The 
<b>LINEMEDIACONTROLDIGIT</b> structure describes a media action to be executed when detecting a digit. It is used as an entry in an array. The 
<a href="https://msdn.microsoft.com/5a4fc83a-6bc9-4081-b374-ddb912fb2242">lineSetMediaControl</a> and 
<a href="https://msdn.microsoft.com/e9273bd6-8dc3-4b45-bf0e-a1a10d78a604">TSPI_lineSetMediaControl</a> functions use this structure.


## -struct-fields




### -field dwDigit

Low-order byte is the digit in whose detection is to trigger a media action. Valid digits depend on the media type.


### -field dwDigitModes

Digit mode(s) to monitor. This member uses one or more of the 
<a href="https://msdn.microsoft.com/d603ea28-2b93-4548-bb16-78e93087f828">LINEDIGITMODE_ Constants</a>.


### -field dwMediaControl

Media control action. This member uses one of the 
<a href="https://msdn.microsoft.com/1e8aeda8-2810-462a-bfba-0296d854d9aa">LINEMEDIACONTROL_ Constants</a>.


## -remarks



This structure may not be extended.

The 
<a href="https://msdn.microsoft.com/5515d510-3827-4da6-975c-ff191bb0ab4e">LINEMEDIACONTROLMEDIA</a> structure defines a triple &lt;digit, digit mode(s), media-control action&gt;. An array of these triples is passed to the 
<a href="https://msdn.microsoft.com/5a4fc83a-6bc9-4081-b374-ddb912fb2242">lineSetMediaControl</a> function to set the media control actions triggered by digits detected on a given call. When a listed digit is detected, then the corresponding action on the media stream is invoked.




## -see-also




<a href="https://msdn.microsoft.com/5515d510-3827-4da6-975c-ff191bb0ab4e">LINEMEDIACONTROLMEDIA</a>



<a href="https://msdn.microsoft.com/e9273bd6-8dc3-4b45-bf0e-a1a10d78a604">TSPI_lineSetMediaControl</a>



<a href="https://msdn.microsoft.com/5a4fc83a-6bc9-4081-b374-ddb912fb2242">lineSetMediaControl</a>
 

 
