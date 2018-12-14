---
UID: NE:websocket._WEB_SOCKET_ACTION_QUEUE
title: WEB_SOCKET_ACTION_QUEUE
author: windows-sdk-content
description: Specifies the action types returned by WebSocketGetAction.
old-location: websock\web_socket_action_queue.htm
tech.root: WebSock
ms.assetid: 59550c5a-a378-4162-a1cc-ed2d05662637
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WEB_SOCKET_ACTION_QUEUE, WEB_SOCKET_ACTION_QUEUE enumeration [Websocket Protocol Component API], WEB_SOCKET_ALL_ACTION_QUEUE, WEB_SOCKET_RECEIVE_ACTION_QUEUE, WEB_SOCKET_SEND_ACTION_QUEUE, websock.web_socket_action_queue, websocket/WEB_SOCKET_ACTION_QUEUE, websocket/WEB_SOCKET_ALL_ACTION_QUEUE, websocket/WEB_SOCKET_RECEIVE_ACTION_QUEUE, websocket/WEB_SOCKET_SEND_ACTION_QUEUE
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: websocket.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
 - Websocket.h
api_name:
 - WEB_SOCKET_ACTION_QUEUE
product: Windows
targetos: Windows
req.typenames: WEB_SOCKET_ACTION_QUEUE
req.redist: 
---

# WEB_SOCKET_ACTION_QUEUE enumeration


## -description


The <b>WEB_SOCKET_ACTION_QUEUE</b> enumeration specifies the action types returned by <a href="https://msdn.microsoft.com/566cff2d-15dd-45c6-bc41-550be1f45cfd">WebSocketGetAction</a>.


## -enum-fields




### -field WEB_SOCKET_SEND_ACTION_QUEUE


<a href="https://msdn.microsoft.com/566cff2d-15dd-45c6-bc41-550be1f45cfd">WebSocketGetAction</a> will return only send-related actions.


### -field WEB_SOCKET_RECEIVE_ACTION_QUEUE


<a href="https://msdn.microsoft.com/566cff2d-15dd-45c6-bc41-550be1f45cfd">WebSocketGetAction</a> will return receive-related actions as well as internal send actions (reply to a ping frame).


### -field WEB_SOCKET_ALL_ACTION_QUEUE


<a href="https://msdn.microsoft.com/566cff2d-15dd-45c6-bc41-550be1f45cfd">WebSocketGetAction</a> will return all actions.


## -see-also




<a href="https://msdn.microsoft.com/46d22fb5-adc3-4d1c-81b8-480f1c6de327">WEB_SOCKET_ACTION</a>



<a href="https://msdn.microsoft.com/e9b90176-c76f-42c2-b378-834a690bfe72">WebSocketCompleteAction</a>



<a href="https://msdn.microsoft.com/566cff2d-15dd-45c6-bc41-550be1f45cfd">WebSocketGetAction</a>
 

 
