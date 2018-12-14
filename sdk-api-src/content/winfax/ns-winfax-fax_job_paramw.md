---
UID: NS:winfax._FAX_JOB_PARAMW
title: FAX_JOB_PARAMW
author: windows-sdk-content
description: The FAX_JOB_PARAM structure contains the information necessary for the fax server to send an individual fax transmission.
old-location: fax\_mfax_fax_job_param_str.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_21yq.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PFAX_JOB_PARAMW, DRT_EMAIL, DRT_INBOX, DRT_NONE, FAX_JOB_PARAM, FAX_JOB_PARAM structure [Fax Service], FAX_JOB_PARAMA, FAX_JOB_PARAMW, JSA_DISCOUNT_PERIOD, JSA_NOW, JSA_SPECIFIC_TIME, PFAX_JOB_PARAM, PFAX_JOB_PARAM structure pointer [Fax Service], _mfax_fax_job_param_str, fax._mfax_fax_job_param_str, winfax/FAX_JOB_PARAM, winfax/FAX_JOB_PARAMA, winfax/FAX_JOB_PARAMW, winfax/PFAX_JOB_PARAM"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winfax.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: FAX_JOB_PARAMW (Unicode) and FAX_JOB_PARAMA (ANSI)
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
 - Winfax.h
api_name:
 - FAX_JOB_PARAM
 - FAX_JOB_PARAMA
 - FAX_JOB_PARAMW
product: Windows
targetos: Windows
req.typenames: FAX_JOB_PARAMW, *PFAX_JOB_PARAMW
req.redist: 
---

# FAX_JOB_PARAMW structure


## -description


The <b>FAX_JOB_PARAM</b> structure contains the information necessary for the fax server to send an individual fax transmission. The structure includes the recipient's fax number, sender and recipient data, an optional billing code, and job scheduling information.

The <b>SizeOfStruct</b>, <b>RecipientNumber</b>, and <b>ScheduleAction</b> members are required; other members are optional.


## -struct-fields




### -field SizeOfStruct

Type: <b>DWORD</b>

Specifies the size, in bytes, of the <b>FAX_JOB_PARAM</b> structure. The calling application must set this member to <b>sizeof(FAX_JOB_PARAM)</b>. This member is required. 


### -field RecipientNumber

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string that specifies the fax number of the recipient of the fax transmission. This member is required. 


### -field RecipientName

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string that specifies the name of the recipient of the fax transmission. 


### -field Tsid

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string that specifies the transmitting station identifier (TSID). This identifier is usually a telephone number. Only printable characters such as English letters, numeric symbols, and punctuation marks (ASCII range 0x20 to 0x7F) can be used in a TSID.


### -field SenderName

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string that specifies the name of the sender who initiated the fax transmission. 


### -field SenderCompany

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string that specifies the company name of the sender who initiated the fax transmission.


### -field SenderDept

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string that specifies the department name of the sender who initiated the fax transmission. 


### -field BillingCode

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string that indicates an application- or server-specific billing code that applies to the fax transmission. The fax server uses the string to generate an entry in the fax event log. Billing codes are optional. 


### -field ScheduleAction

Type: <b>DWORD</b>

Specifies a DWORD variable that indicates when to send the fax. This member is required, and can be one of the following predefined job scheduling actions. 



#### JSA_NOW

Send the fax as soon as a device is available. 



#### JSA_SPECIFIC_TIME

Send the fax at the time specified by the <b>ScheduleTime</b> member. 



#### JSA_DISCOUNT_PERIOD

Send the fax during the discount rate period. Call the <a href="https://msdn.microsoft.com/c29f0eaf-39a5-45e2-afb9-010494552969">FaxGetConfiguration</a> function to retrieve the discount period for the fax server. 


### -field ScheduleTime

Type: <b><a href="https://msdn.microsoft.com/f77cdf86-0f97-4a89-b565-95b46fa7d65b">SYSTEMTIME</a></b>

If the <b>ScheduleAction</b> member is equal to the value <b>JSA_SPECIFIC_TIME</b>, specifies a <a href="https://msdn.microsoft.com/f77cdf86-0f97-4a89-b565-95b46fa7d65b">SYSTEMTIME</a> structure that contains the date and time to send the fax. The time specified must be expressed in UTC.


### -field DeliveryReportType

Type: <b>DWORD</b>

Specifies a <b>DWORD</b> variable that indicates the type of email delivery report (DR) or nondelivery report (NDR) that the fax server should generate. This member can be one of the following predefined delivery report types. 



#### DRT_NONE

Do not send a DR or an NDR to the sender of the fax transmission. 



#### DRT_EMAIL

Send the DR or NDR in an email message to the sender of the fax transmission (supported in Windows Server 2003 and later). 



#### DRT_INBOX

Send the DR or NDR in email to the sender's local personal information store. 


### -field DeliveryReportAddress

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string. If the <b>DeliveryReportType</b> member is equal to <b>DRT_EMAIL</b>, the string is the address to which the DR or NDR should be sent. If the <b>DeliveryReportType</b> member is equal to <b>DRT_NONE</b>, this member must be <b>NULL</b>. 


### -field DocumentName

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string to associate with the fax document. This is the user-friendly name that appears in the print spooler.


### -field CallHandle

Type: <b>HCALL</b>

Reserved, and should be <b>NULL</b>.


### -field Reserved

Type: <b>DWORD_PTR[3]</b>

This member is reserved for future use by Microsoft. It must be set to zero. 


##### - DeliveryReportType.DRT_EMAIL

Send the DR or NDR in an email message to the sender of the fax transmission (supported in Windows Server 2003 and later). 


##### - DeliveryReportType.DRT_INBOX

Send the DR or NDR in email to the sender's local personal information store. 


##### - DeliveryReportType.DRT_NONE

Do not send a DR or an NDR to the sender of the fax transmission. 


##### - ScheduleAction.JSA_DISCOUNT_PERIOD

Send the fax during the discount rate period. Call the <a href="https://msdn.microsoft.com/c29f0eaf-39a5-45e2-afb9-010494552969">FaxGetConfiguration</a> function to retrieve the discount period for the fax server. 


##### - ScheduleAction.JSA_NOW

Send the fax as soon as a device is available. 


##### - ScheduleAction.JSA_SPECIFIC_TIME

Send the fax at the time specified by the <b>ScheduleTime</b> member. 


## -remarks



A fax client application passes the <b>FAX_JOB_PARAM</b> structure in a call to the <a href="https://msdn.microsoft.com/bbf8def4-4af0-4315-94f9-860f9db1eefa">FaxSendDocument</a> function to inform the fax server how and when to send the fax transmission. For more information, see <a href="https://msdn.microsoft.com/99331570-b396-4ed8-b2f4-3db883be0130">Sending a Fax to One Recipient (Win32 Environment)</a>.




## -see-also




<a href="https://msdn.microsoft.com/be81e221-4aba-4c63-9640-337bee49fdb4">Fax Service Client API Structures</a>



<a href="https://msdn.microsoft.com/cbc79dc5-d0ca-418d-8572-64b0a582056f">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/46eb9960-1d07-4792-83d6-d2f5948e05e9">FaxCompleteJobParams</a>



<a href="https://msdn.microsoft.com/c29f0eaf-39a5-45e2-afb9-010494552969">FaxGetConfiguration</a>



<a href="https://msdn.microsoft.com/bbf8def4-4af0-4315-94f9-860f9db1eefa">FaxSendDocument</a>



<a href="https://msdn.microsoft.com/f77cdf86-0f97-4a89-b565-95b46fa7d65b">SYSTEMTIME</a>



<a href="_tapi2_linemakecall">lineMakeCall</a>
 

 
