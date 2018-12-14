---
UID: NF:locationapi.ICivicAddressReport.GetPostalCode
title: ICivicAddressReport::GetPostalCode
author: windows-sdk-content
description: Retrieves the postal code.
old-location: winlocation_com_ref\icivicaddressreport_getpostalcode.htm
tech.root: locationapi
ms.assetid: 1580a1b9-1503-43d8-af1c-3b2ba8e9f81a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetPostalCode, GetPostalCode method [WinLocation], GetPostalCode method [WinLocation],ICivicAddressReport interface, ICivicAddressReport interface [WinLocation],GetPostalCode method, ICivicAddressReport.GetPostalCode, ICivicAddressReport::GetPostalCode, WinLocation_COM_Ref.icivicaddressreport_getpostalcode, locationapi/ICivicAddressReport::GetPostalCode
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: locationapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only],Windows 7
req.target-min-winversvr: None supported
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
req.dll: LocationAPI.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - LocationAPI.dll
api_name:
 - ICivicAddressReport.GetPostalCode
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ICivicAddressReport::GetPostalCode


## -description


<p class="CCE_Message">[The Win32 Location API is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions. Instead, use the <a href="https://msdn.microsoft.com/fd40bf4a-c59a-43a4-ab01-c671a8a41731">Windows.Devices.Geolocation</a>API.
]

Retrieves the postal code.


## -parameters




### -param pbstrPostalCode [out]

Address of a <b>BSTR</b> that receives the postal code.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/ba8c66cb-be94-4649-ada9-620ed3b35516">ICivicAddressReport</a>
 

 
