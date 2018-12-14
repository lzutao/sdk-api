---
UID: NF:timezoneapi.GetDynamicTimeZoneInformationEffectiveYears
title: GetDynamicTimeZoneInformationEffectiveYears function
author: windows-sdk-content
description: Gets a range, expressed in years, for which a DYNAMIC_TIME_ZONE_INFORMATION has valid entries.
old-location: base\getdynamictimezoneinformationeffectiveyears.htm
tech.root: sysinfo
ms.assetid: 6705BF71-9FF9-4D1F-B34B-752D9C83C964
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: GetDynamicTimeZoneInformationEffectiveYears, GetDynamicTimeZoneInformationEffectiveYears function, base.getdynamictimezoneinformationeffectiveyears, timezoneapi/GetDynamicTimeZoneInformationEffectiveYears
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: timezoneapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
 - API-MS-Win-Core-TimeZone-l1-1-0.dll
 - KernelBase.dll
 - MinKernelBase.dll
api_name:
 - GetDynamicTimeZoneInformationEffectiveYears
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# GetDynamicTimeZoneInformationEffectiveYears function


## -description


Gets a range, expressed in years, for which a <a href="https://msdn.microsoft.com/d60b1212-26bc-4fad-afce-9bd9062ca5b0">DYNAMIC_TIME_ZONE_INFORMATION</a> has valid entries. Use the returned value to identify the specific years to request when calling <a href="https://msdn.microsoft.com/5bd29a25-98f0-439e-be88-8011bbf98926">GetTimeZoneInformationForYear</a> to retrieve time zone information for a time zone that experiences annual boundary changes due to daylight saving time adjustments.


## -parameters




### -param lpTimeZoneInformation [in]

Specifies settings for  a time zone and dynamic daylight saving time.


### -param FirstYear [out]

The year that marks the beginning of the range to pass to <a href="https://msdn.microsoft.com/5bd29a25-98f0-439e-be88-8011bbf98926">GetTimeZoneInformationForYear</a>.


### -param LastYear [out]

The year that marks the end of the range to pass to <a href="https://msdn.microsoft.com/5bd29a25-98f0-439e-be88-8011bbf98926">GetTimeZoneInformationForYear</a>.


## -returns



<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
</dl>
</td>
<td width="60%">
The operation succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b> ERROR_FILE_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
The system cannot find the effective years.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
One of the parameter values is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>Any other value</dt>
</dl>
</td>
<td width="60%">
The operation failed.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/d60b1212-26bc-4fad-afce-9bd9062ca5b0">DYNAMIC_TIME_ZONE_INFORMATION</a>



<a href="https://msdn.microsoft.com/EBB2366A-86FE-4764-B7F9-5D305993CE0A">EnumDynamicTimeZoneInformation</a>
 

 
