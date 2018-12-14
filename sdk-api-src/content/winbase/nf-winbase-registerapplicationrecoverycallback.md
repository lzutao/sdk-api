---
UID: NF:winbase.RegisterApplicationRecoveryCallback
title: RegisterApplicationRecoveryCallback function
author: windows-sdk-content
description: Registers the active instance of an application for recovery.
old-location: recovery\registerapplicationrecoverycallback.htm
tech.root: Recovery
ms.assetid: 4ff73c2c-a941-4626-ae40-cafbe6e50644
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: RegisterApplicationRecoveryCallback, RegisterApplicationRecoveryCallback function [Recovery], base.registerapplicationrecoverycallback, recovery.registerapplicationrecoverycallback, winbase/RegisterApplicationRecoveryCallback
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winbase.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
api_name:
 - RegisterApplicationRecoveryCallback
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# RegisterApplicationRecoveryCallback function


## -description


Registers the active instance of an application for recovery.


## -parameters




### -param pRecoveyCallback [in]

A pointer to the recovery callback function. For more information, see <a href="https://msdn.microsoft.com/573b1adb-9d9e-4a58-8d02-2addb93626da">ApplicationRecoveryCallback</a>.


### -param pvParameter [in, optional]

A pointer to a variable to be passed to the callback function. Can be <b>NULL</b>.


### -param dwPingInterval [in]

The recovery ping interval, in milliseconds. By default, the interval is 5 seconds (RECOVERY_DEFAULT_PING_INTERVAL). The maximum interval is 5 minutes. If you specify zero, the default interval is used. 

You must call the <a href="https://msdn.microsoft.com/9c765f72-10ad-4d16-a9e5-d73ea5c4f59b">ApplicationRecoveryInProgress</a> function within the specified interval to indicate to ARR that you are still actively recovering; otherwise, WER terminates recovery. Typically, you perform recovery in a loop with each iteration lasting no longer than the ping interval. Each iteration performs a block of recovery work followed by a call to <b>ApplicationRecoveryInProgress</b>. Since you also use <b>ApplicationRecoveryInProgress</b> to determine if the user wants to cancel recovery, you should consider a smaller interval, so you do not perform a lot of work unnecessarily.


### -param dwFlags [in]

Reserved for future use. Set to zero.


## -returns



This function returns <b>S_OK</b> on success or one of the following error codes.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
Internal error; the registration failed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The ping interval cannot be more than five minutes.

</td>
</tr>
</table>
 




## -remarks



If the  application encounters an unhandled exception or becomes unresponsive, Windows Error Reporting (WER) calls the specified recovery callback. You should use the callback to save data and state information. You can use the information if you also call  the <a href="https://msdn.microsoft.com/f4cd25b3-2aee-460f-9f9f-b45ecded094f">RegisterApplicationRestart</a> function to request that WER restart the application.

WER will not call your recovery callback if an installer wants to  update a component of your application. To save data and state information in the update case, you should handle the <a href="https://msdn.microsoft.com/7ad73444-f1f6-4b73-8450-0580b146a5a6">WM_QUERYENDSESSION</a> and <a href="https://msdn.microsoft.com/9bf04f24-da1e-4680-a47b-28e9c500635e">WM_ENDSESSION</a> messages. For details, see each message. The timeout for responding to these messages is five seconds. Most of the available recovery time is in the <a href="https://msdn.microsoft.com/en-us/library/ms632617(v=VS.85).aspx">WM_CLOSE</a> message for which you have 30 seconds.

A console application that can be updated uses the CTRL_C_EVENT notification to initiate recovery (for details, see the <a href="https://msdn.microsoft.com/library/ms683242(v=VS.85).aspx">HandlerRoutine</a> callback function). The timeout for the handler to complete is 30 seconds.

Applications should consider saving data and state information on a periodic bases to shorten the amount of time required for recovery.




## -see-also




<a href="https://msdn.microsoft.com/573b1adb-9d9e-4a58-8d02-2addb93626da">ApplicationRecoveryCallback</a>



<a href="https://msdn.microsoft.com/9c765f72-10ad-4d16-a9e5-d73ea5c4f59b">ApplicationRecoveryInProgress</a>



<a href="https://msdn.microsoft.com/f4cd25b3-2aee-460f-9f9f-b45ecded094f">RegisterApplicationRestart</a>



<a href="https://msdn.microsoft.com/473e24d6-fddb-4935-b454-8cddfb53a02a">UnregisterApplicationRecoveryCallback</a>
 

 
