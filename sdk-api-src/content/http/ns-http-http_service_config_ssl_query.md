---
UID: NS:http._HTTP_SERVICE_CONFIG_SSL_QUERY
title: HTTP_SERVICE_CONFIG_SSL_QUERY
author: windows-sdk-content
description: Used to specify a particular record to query in the SSL configuration store.
old-location: http\http_service_config_ssl_query.htm
tech.root: http
ms.assetid: 733b451a-d35b-4b83-ba49-0529309cd99b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PHTTP_SERVICE_CONFIG_SSL_QUERY, HTTP_SERVICE_CONFIG_SSL_QUERY, HTTP_SERVICE_CONFIG_SSL_QUERY structure [HTTP], PHTTP_SERVICE_CONFIG_SSL_QUERY, PHTTP_SERVICE_CONFIG_SSL_QUERY structure pointer [HTTP], _http_http_service_config_ssl_query, http.http_service_config_ssl_query, http/HTTP_SERVICE_CONFIG_SSL_QUERY, http/PHTTP_SERVICE_CONFIG_SSL_QUERY"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: http.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - Http.h
api_name:
 - HTTP_SERVICE_CONFIG_SSL_QUERY
product: Windows
targetos: Windows
req.typenames: HTTP_SERVICE_CONFIG_SSL_QUERY, *PHTTP_SERVICE_CONFIG_SSL_QUERY
req.redist: 
---

# HTTP_SERVICE_CONFIG_SSL_QUERY structure


## -description


The 
<b>HTTP_SERVICE_CONFIG_SSL_QUERY</b> structure is used to specify a particular record to query in the SSL configuration store. It is passed to the 
<a href="https://msdn.microsoft.com/bbd2c3c4-d2d0-4590-9b5c-6916b91600cd">HttpQueryServiceConfiguration</a> function using the <i>pInputConfigInfo</i> parameter when the <i>ConfigId</i> parameter is set to <b>HttpServiceConfigSSLCertInfo</b>.


## -struct-fields




### -field QueryDesc

One of the  following values from the <a href="https://msdn.microsoft.com/63b2503f-7e71-4c62-8e9c-ad0f5103a9e8">HTTP_SERVICE_CONFIG_QUERY_TYPE</a> enumeration. 







#### HttpServiceConfigQueryExact

Returns a single SSL record.



#### HttpServiceConfigQueryNext

Returns a sequence of SSL records in a sequence of calls, as controlled by the <i>dwToken</i> parameter.


### -field KeyDesc

If the <i>QueryDesc</i> parameter is equal to <b>HttpServiceConfigQueryExact</b>, then <i>KeyDesc</i> should contain an 
<a href="https://msdn.microsoft.com/67231fa5-69eb-4353-8c3c-326ec9095554">HTTP_SERVICE_CONFIG_SSL_KEY</a> structure that identifies the SSL certificate record queried. If the <i>QueryDesc</i> parameter is equal to HTTPServiceConfigQueryNext, then <i>KeyDesc</i> is ignored.


### -field dwToken

If the <i>QueryDesc</i> parameter is equal to <b>HTTPServiceConfigQueryNext</b>, then <i>dwToken</i> must be equal to zero on the first call to the 
<a href="https://msdn.microsoft.com/bbd2c3c4-d2d0-4590-9b5c-6916b91600cd">HttpQueryServiceConfiguration</a> function, one on the second call, two on the third call, and so forth until all SSL certificate records are returned, at which point 
<b>HttpQueryServiceConfiguration</b> returns ERROR_NO_MORE_ITEMS. 




If the <i>QueryDesc</i> parameter is equal to <b>HttpServiceConfigQueryExact</b>, then <i>dwToken</i> is ignored.


## -see-also




<a href="https://msdn.microsoft.com/63b2503f-7e71-4c62-8e9c-ad0f5103a9e8">HTTP_SERVICE_CONFIG_QUERY_TYPE</a>



<a href="https://msdn.microsoft.com/23adda0b-907d-4804-9c12-e549af4f18c4">HTTP_SERVICE_CONFIG_SSL_SET</a>



<a href="https://msdn.microsoft.com/bbd2c3c4-d2d0-4590-9b5c-6916b91600cd">HttpQueryServiceConfiguration</a>
 

 
