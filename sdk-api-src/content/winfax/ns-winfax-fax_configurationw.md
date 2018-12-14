---
UID: NS:winfax._FAX_CONFIGURATIONW
title: FAX_CONFIGURATIONW
author: windows-sdk-content
description: The FAX_CONFIGURATION structure contains information about the global configuration settings of a fax server.
old-location: fax\_mfax_fax_configuration_str.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxlegacy_14aa.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PFAX_CONFIGURATIONW, FAX_CONFIGURATION, FAX_CONFIGURATION structure [Fax Service], FAX_CONFIGURATIONA, FAX_CONFIGURATIONW, PFAX_CONFIGURATION, PFAX_CONFIGURATION structure pointer [Fax Service], _mfax_fax_configuration_str, fax._mfax_fax_configuration_str, winfax/FAX_CONFIGURATION, winfax/FAX_CONFIGURATIONA, winfax/FAX_CONFIGURATIONW, winfax/PFAX_CONFIGURATION"
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
req.unicode-ansi: FAX_CONFIGURATIONW (Unicode) and FAX_CONFIGURATIONA (ANSI)
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
 - FAX_CONFIGURATION
 - FAX_CONFIGURATIONA
 - FAX_CONFIGURATIONW
product: Windows
targetos: Windows
req.typenames: FAX_CONFIGURATIONW, *PFAX_CONFIGURATIONW
req.redist: 
---

# FAX_CONFIGURATIONW structure


## -description


The <b>FAX_CONFIGURATION</b> structure contains information about the global configuration settings of a fax server. The structure includes data on retransmission, branding, archive, and cover page settings; discount rate periods; and the status of the fax server queue.


## -struct-fields




### -field SizeOfStruct

Type: <b>DWORD</b>

Specifies the size, in bytes, of the <b>FAX_CONFIGURATION</b> structure. The calling application must set this member to <b>sizeof(FAX_CONFIGURATION)</b> before it calls the <a href="https://msdn.microsoft.com/e99d5254-4008-411a-ae56-8b0cbe7a4933">FaxSetConfiguration</a> function.


### -field Retries

Type: <b>DWORD</b>

Specifies a <b>DWORD</b> variable that indicates the number of times the fax server will attempt to retransmit an outgoing fax if the initial transmission fails.


### -field RetryDelay

Type: <b>DWORD</b>

Specifies a <b>DWORD</b> variable that indicates the number of minutes that will elapse between retransmission attempts by the fax server.


### -field DirtyDays

Type: <b>DWORD</b>

Specifies a <b>DWORD</b> variable that indicates the number of days the fax server will retain an unsent job in the fax job queue. A transmission might not be sent, for example, if an invalid fax number or date is specified, or if the sending device receives a busy signal multiple times.


### -field Branding

Type: <b>BOOL</b>

Specifies a Boolean variable that indicates whether the fax server should generate a brand (banner) at the top of outgoing fax transmissions. If this member is <b>TRUE</b>, the fax server generates a brand that contains transmission-related information like the transmitting station identifier, date, time, and page count.


### -field UseDeviceTsid

Type: <b>BOOL</b>

Specifies a Boolean variable that indicates whether the fax server will use the device's transmitting station identifier instead of the value specified in the <b>Tsid</b> member of the <a href="https://msdn.microsoft.com/d589a255-abe2-49d5-b593-3a60cdaf61eb">FAX_JOB_PARAM</a> structure. If this member is <b>TRUE</b>, the server uses the device's transmitting station identifier.


### -field ServerCp

Type: <b>BOOL</b>

Specifies a Boolean variable that indicates whether fax client applications can include a user-designed cover page with the fax transmission. If this member is <b>TRUE</b>, the client must use a common cover page stored on the fax server. If this member is <b>FALSE</b>, the client can use a personal cover page file.


### -field PauseServerQueue

Type: <b>BOOL</b>

Specifies a Boolean variable that indicates whether the fax server has paused the fax job queue. If this member is <b>TRUE</b>, the queue has been paused.


### -field StartCheapTime

Type: <b><a href="https://msdn.microsoft.com/5d045860-463f-444c-a86a-0e7fab3b3ebc">FAX_TIME</a></b>

Specifies a <a href="https://msdn.microsoft.com/5d045860-463f-444c-a86a-0e7fab3b3ebc">FAX_TIME</a> structure that indicates the hour and minute at which the discount period begins. The discount period applies only to outgoing transmissions.


### -field StopCheapTime

Type: <b><a href="https://msdn.microsoft.com/5d045860-463f-444c-a86a-0e7fab3b3ebc">FAX_TIME</a></b>

Specifies a <a href="https://msdn.microsoft.com/5d045860-463f-444c-a86a-0e7fab3b3ebc">FAX_TIME</a> structure that indicates the hour and minute at which the discount period ends. The discount period applies only to outgoing transmissions.


### -field ArchiveOutgoingFaxes

Type: <b>BOOL</b>

Specifies a Boolean variable that indicates whether the fax server should archive outgoing fax transmissions. If this member is <b>TRUE</b>, the server archives outgoing transmissions in the directory specified by the <b>ArchiveDirectory</b> member.


### -field ArchiveDirectory

Type: <b>LPCTSTR</b>

Pointer to a constant null-terminated character string that contains the fully qualified path of the directory in which outgoing fax transmissions will be archived. The path can be a UNC path or a path beginning with a drive letter. The fax server ignores this member if the <b>ArchiveOutgoingFaxes</b> member is <b>FALSE</b>. This member can be <b>NULL</b> if the <b>ArchiveOutgoingFaxes</b> member is <b>FALSE</b>.


### -field Reserved

 




#### - InboundProfile

Type: <b>LPCSTR</b>

The inbound routing profile used for email.


## -remarks



The fax client application passes the <b>FAX_CONFIGURATION</b> structure in a call to the <a href="https://msdn.microsoft.com/e99d5254-4008-411a-ae56-8b0cbe7a4933">FaxSetConfiguration</a> function to change the global configuration settings for the fax server of interest. If the application calls the <a href="https://msdn.microsoft.com/c29f0eaf-39a5-45e2-afb9-010494552969">FaxGetConfiguration</a> function, it returns the current settings in a <b>FAX_CONFIGURATION</b> structure. For more information, see <a href="https://msdn.microsoft.com/49416909-d475-4c76-ae2a-bd3c39611b32">Fax Server Configuration Management</a>.




## -see-also




<a href="https://msdn.microsoft.com/d589a255-abe2-49d5-b593-3a60cdaf61eb">FAX_JOB_PARAM</a>



<a href="https://msdn.microsoft.com/5d045860-463f-444c-a86a-0e7fab3b3ebc">FAX_TIME</a>



<a href="https://msdn.microsoft.com/be81e221-4aba-4c63-9640-337bee49fdb4">Fax Service Client API Structures</a>



<a href="https://msdn.microsoft.com/cbc79dc5-d0ca-418d-8572-64b0a582056f">Fax Service Client API for Windows 2000</a>



<a href="https://msdn.microsoft.com/c29f0eaf-39a5-45e2-afb9-010494552969">FaxGetConfiguration</a>



<a href="https://msdn.microsoft.com/e99d5254-4008-411a-ae56-8b0cbe7a4933">FaxSetConfiguration</a>
 

 
