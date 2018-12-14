---
UID: NS:webservices._WS_XML_TIMESPAN_TEXT
title: WS_XML_TIMESPAN_TEXT
author: windows-sdk-content
description: Represents a time span formatted as the text &#0034;[+|-][d?.]HH:mm:ss[.fffffff]&#0034; d is a series of digits representing the day.
old-location: wsw\ws_xml_timespan_text.htm
tech.root: wsw
ms.assetid: 6b502748-bfe1-4a8c-97e9-f8ae97c96b01
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WS_XML_TIMESPAN_TEXT, WS_XML_TIMESPAN_TEXT structure [Web Services for Windows], webservices/WS_XML_TIMESPAN_TEXT, wsw.ws_xml_timespan_text
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: webservices.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - WebServices.h
api_name:
 - WS_XML_TIMESPAN_TEXT
product: Windows
targetos: Windows
req.typenames: WS_XML_TIMESPAN_TEXT
req.redist: 
---

# WS_XML_TIMESPAN_TEXT structure


## -description


Represents a time span formatted as the text "[+|-][d?.]HH:mm:ss[.fffffff]"
        <ul>
<li>d is a series of digits representing the day.
          </li>
<li>HH is a two digit number representing the hour of the day, from to 0 to 23.
          </li>
<li>mm is a two digit number representing the minute of the hour, from to 0 to 59.
          </li>
<li>ss is a two digit number representing the second of the minute, from to 0 to 59.
          </li>
<li>fffffff is up to 7 decimal digits representing the fraction of a second.
        </li>
</ul>



## -struct-fields




### -field text

The base type for all types that derive from <a href="https://msdn.microsoft.com/430edd13-b664-4e10-8d61-ffa6a01dcb90">WS_XML_TEXT</a>.
        


### -field value

The timespan.
