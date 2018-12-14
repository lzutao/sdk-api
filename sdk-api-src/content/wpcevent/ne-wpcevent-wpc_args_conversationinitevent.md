---
UID: NE:wpcevent.tagWPC_ARGS_CONVERSATIONINITEVENT
title: WPC_ARGS_CONVERSATIONINITEVENT
author: windows-sdk-content
description: Indicates information about initiating a conversation.
old-location: parcon\wpc_args_conversationinitevent.htm
tech.root: parcon
ms.assetid: 024e64b0-6b22-4e1e-a37c-d3e7884d295a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WPC_ARGS_CONVERSATIONINITEVENT, WPC_ARGS_CONVERSATIONINITEVENT enumeration, WPC_ARGS_CONVERSATIONINITEVENT_ACCOUNTNAME, WPC_ARGS_CONVERSATIONINITEVENT_APPNAME, WPC_ARGS_CONVERSATIONINITEVENT_APPVERSION, WPC_ARGS_CONVERSATIONINITEVENT_CARGS, WPC_ARGS_CONVERSATIONINITEVENT_CONVID, WPC_ARGS_CONVERSATIONINITEVENT_REASON, WPC_ARGS_CONVERSATIONINITEVENT_RECIPCOUNT, WPC_ARGS_CONVERSATIONINITEVENT_RECIPIENT, WPC_ARGS_CONVERSATIONINITEVENT_REQUESTINGIP, WPC_ARGS_CONVERSATIONINITEVENT_SENDER, parcon.wpc_args_conversationinitevent, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_ACCOUNTNAME, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_APPNAME, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_APPVERSION, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_CARGS, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_CONVID, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_REASON, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_RECIPCOUNT, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_RECIPIENT, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_REQUESTINGIP, wpcevent/WPC_ARGS_CONVERSATIONINITEVENT_SENDER
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: wpcevent.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Wpcevent.h
api_name:
 - WPC_ARGS_CONVERSATIONINITEVENT
product: Windows
targetos: Windows
req.typenames: WPC_ARGS_CONVERSATIONINITEVENT
req.redist: 
---

# WPC_ARGS_CONVERSATIONINITEVENT enumeration


## -description


Indicates information about initiating a conversation.


## -enum-fields




### -field WPC_ARGS_CONVERSATIONINITEVENT_APPNAME

The name of the application used for starting the conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_APPVERSION

The version of the application used for starting the conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_ACCOUNTNAME

The account name used for starting the conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_CONVID

The conversation identifier used for starting the conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_REQUESTINGIP

The IP address of the computer starting the conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_SENDER

The sender who is starting the conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_REASON

The reason given for starting the conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_RECIPCOUNT

The number of recipients included in starting the conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_RECIPIENT

The recipient of the started conversation.


### -field WPC_ARGS_CONVERSATIONINITEVENT_CARGS

The arguments used for starting the conversation.
