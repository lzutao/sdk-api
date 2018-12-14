---
UID: NF:tspi.TSPI_lineSetStatusMessages
title: TSPI_lineSetStatusMessages function
author: windows-sdk-content
description: The TSPI_lineSetStatusMessages function enables TAPI to specify which notification messages the service provider should generate for events related to status changes for the specified line or any of its addresses.
old-location: tspi\tspi_linesetstatusmessages.htm
tech.root: tapi
ms.assetid: 546c4f6e-6bda-4b4b-91ed-51d0b64af677
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: TSPI_lineSetStatusMessages, TSPI_lineSetStatusMessages function [TAPI 2.2], _tspi_tspi_linesetstatusmessages, tspi.tspi_linesetstatusmessages, tspi/TSPI_lineSetStatusMessages
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: tspi.h
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
 - UserDefined
api_location:
 - Tspi.h
api_name:
 - TSPI_lineSetStatusMessages
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# TSPI_lineSetStatusMessages function


## -description


The 
<b>TSPI_lineSetStatusMessages</b> function enables TAPI to specify which notification messages the service provider should generate for events related to status changes for the specified line or any of its addresses.


## -parameters




### -param hdLine

The handle to the line device for which the new filter is to be set.


### -param dwLineStates

A bit array that identifies for which line device status changes a message is to be sent to TAPI. This parameter uses one of the 
<a href="https://msdn.microsoft.com/41e8a777-a57a-4d6c-850f-e21b58081b0d">LINEDEVSTATE_ constants</a>.


### -param dwAddressStates

A bit array that identifies for which address status changes a message is to be sent to TAPI. This parameter uses one of the 
<a href="https://msdn.microsoft.com/f06140d0-f41a-4228-93c5-21d609af5473">LINEADDRESSSTATE_ constants</a>.


## -returns



Returns zero if the function succeeds, or an error number if an error occurs. Possible return values are as follows:

LINEERR_INVALADDRESSSTATE, LINEERR_OPERATIONUNAVAIL, LINEERR_INVALLINEHANDLE, LINEERR_OPERATIONFAILED, LINEERR_INVALLINESTATE, LINEERR_RESOURCEUNAVAIL, LINEERR_NOMEM.




## -remarks



The service provider returns LINEERR_INVALLINESTATE if the <i>dwLineStates</i> parameter contains one or more bits that are not 
<a href="https://msdn.microsoft.com/41e8a777-a57a-4d6c-850f-e21b58081b0d">LINEDEVSTATE_ constants</a>.

 Telephony defines a number of messages that notify applications about events occurring on lines and addresses. The sets of all change messages in which all applications are interested can be much smaller than the set of possible messages. This procedure allows TAPI to tell the service provider the reduced set of messages to deliver. The service provider delivers all of the messages it supports, within the specified set. It is permitted to deliver more (they are filtered out by TAPI), but is discouraged from doing so for performance reasons. If TAPI requests delivery of a particular message type that is not produced by the provider, the provider nevertheless accepts the request but simply does not produce the message. By default, address and line status reporting is initially disabled for a line.

This function differs from the corresponding TAPI function as follows: (1) The set of messages requested is the union of all sets requested by applications at the TAPI level. (2) The message set is neither reduced nor augmented by ownership (because there is no concept of ownership at the TSPI level) (3) The set is advisory in the sense that the service provider is required to forward at least the indicated set of messages but is permitted to forward a larger set.

Device state changes regarding Open and Close are not reported, because at the TSPI level there is only one outstanding Open at a time.




## -see-also




<a href="https://msdn.microsoft.com/f06140d0-f41a-4228-93c5-21d609af5473">LINEADDRESSSTATE_ Constants</a>



<a href="https://msdn.microsoft.com/41e8a777-a57a-4d6c-850f-e21b58081b0d">LINEDEVSTATE_ Constants</a>



<a href="https://msdn.microsoft.com/0015b67d-229d-412f-aea8-ec97a28813b9">LINE_ADDRESSSTATE</a>



<a href="https://msdn.microsoft.com/0344151e-3f40-472d-84c2-906291777da6">LINE_CLOSE</a>



<a href="https://msdn.microsoft.com/6e59a7a7-660c-493f-ae0f-0c46a446c4be">LINE_LINEDEVSTATE</a>
 

 
