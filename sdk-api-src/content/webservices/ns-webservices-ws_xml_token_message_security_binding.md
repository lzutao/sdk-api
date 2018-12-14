---
UID: NS:webservices._WS_XML_TOKEN_MESSAGE_SECURITY_BINDING
title: WS_XML_TOKEN_MESSAGE_SECURITY_BINDING
author: windows-sdk-content
description: The security binding subtype for specifying the use of a security token that is already available to the application in XML form.
old-location: wsw\ws_xml_token_message_security_binding.htm
tech.root: wsw
ms.assetid: 5ca1e67a-11f5-44bb-afe8-c934837d711b
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WS_XML_TOKEN_MESSAGE_SECURITY_BINDING, WS_XML_TOKEN_MESSAGE_SECURITY_BINDING structure [Web Services for Windows], webservices/WS_XML_TOKEN_MESSAGE_SECURITY_BINDING, wsw.ws_xml_token_message_security_binding
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
 - WS_XML_TOKEN_MESSAGE_SECURITY_BINDING
product: Windows
targetos: Windows
req.typenames: WS_XML_TOKEN_MESSAGE_SECURITY_BINDING
req.redist: 
---

# WS_XML_TOKEN_MESSAGE_SECURITY_BINDING structure


## -description


The security binding subtype for specifying the use of a security
token that is already available to the application in XML form.  The
security token that is supplied by the application in this binding is
presented to a service in a WS-Security header according to the
bindingUsage specified.  This security binding may be included in a 
<a href="https://msdn.microsoft.com/b9490f00-877c-4d9f-b361-eaca343cdee0">security description</a> only on the
client side.
            

This security binding is not supported with the <a href="https://msdn.microsoft.com/554cc239-feab-4262-9821-6478a3d93ffc">WS_NAMEDPIPE_CHANNEL_BINDING</a>.

Although this binding can be used with any token available in XML
form, this is commonly used in <a href="https://msdn.microsoft.com/574496df-95dc-45f7-8c42-e646aec12e69">federation
scenarios</a>.  For example, a client side token provider such as
CardSpace may be used to get a token from a security token service,
and that token may then be presented to a Web Service using this
security binding.
            

Security note: As with other security tokens and credentials, the
application is in charge of the risk assessment decision to disclose a
given XML token (supplied by the application in a 
<a href="https://msdn.microsoft.com/b9490f00-877c-4d9f-b361-eaca343cdee0">security description</a>) to a given
server (supplied by the application when 
<a href="https://msdn.microsoft.com/a7226194-0974-4f3c-b92d-78a93e86eea5">opening the channel</a>).  In particular, the
application should consider the threat that the server might use the
XML token it receives from the client, in turn, to pretend to be the
client to a 3rd party.  For this threat, the following mitigations
exist: (A) the server authentication process makes sure that the
message (and hence the token) is sent only to a server that can speak
for the address specified by the client application; (B) keyless
(bearer) tokens are typically usable only at one server (e.g.,
contoso.com gains little from passing on a contoso.com
username/password token to another site -- the application security
design should make sure this property holds); (C) symmetric keyed
tokens are unusable at any server that doesn't share the same
symmetric key; (D) asymmetric keyed tokens will sign the timestamp and
the 'To' header, limiting their applicability to the intended 'To' for
a narrow time duration.
            

With this security binding, no security binding properties may be specified:
            


## -struct-fields




### -field binding

The base type from which this security binding subtype and all other security binding subtypes derive.
                


### -field bindingUsage

How the security token corresponding to this security binding should be bound to a message.
                

Only <a href="https://msdn.microsoft.com/2f19877f-b79b-43c3-a3f5-93dd2940d499">WS_SUPPORTING_MESSAGE_SECURITY_USAGE</a> is
supported.  With this usage, this security binding provides client
authentication, but not message protection (such as signing,
encryption, replay detection).  Thus, this binding must be used
together with another security binding such as the <a href="https://msdn.microsoft.com/078efc1d-a1bc-4035-919c-f927a8ceb8e6">WS_SSL_TRANSPORT_SECURITY_BINDING</a> that provides a protected
channel.
                


### -field xmlToken

The XML security token to be used.  This token may be created using <a href="https://msdn.microsoft.com/1d82c6c3-2bcf-4883-aed7-1a163bbb2228">WsCreateXmlSecurityToken</a> or obtained from a security token
service using <a href="https://msdn.microsoft.com/ee754a7d-73a9-49ae-afc7-b443fbbe0cce">WsRequestSecurityToken</a>.  When this binding is
used for creating a channel, a copy of the supplied token is made and
kept for internal use -- the application continues to own the supplied
token and is responsible for deleting it with <a href="https://msdn.microsoft.com/7f9500a8-b54f-4967-8f8d-9f8770d3dd60">WsFreeSecurityToken</a> any time after the channel creation call
returns.
                
