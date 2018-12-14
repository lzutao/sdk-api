---
UID: NC:winwlx.PWLX_DIALOG_BOX_PARAM
title: PWLX_DIALOG_BOX_PARAM
author: windows-sdk-content
description: Called by GINA to initialize dialog box controls and then create a modal dialog box from a dialog box template resource.
old-location: security\wlxdialogboxparam.htm
tech.root: secauthn
ms.assetid: 0b4543e1-066b-4d19-9b15-90d966d25154
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PWLX_DIALOG_BOX_PARAM, PWLX_DIALOG_BOX_PARAM callback, WlxDialogBoxParam, WlxDialogBoxParam callback function [Security], _gina_wlxdialogboxparam, security.wlxdialogboxparam, winwlx/WlxDialogBoxParam
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: winwlx.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
 - UserDefined
api_location:
 - winwlx.h
api_name:
 - WlxDialogBoxParam
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PWLX_DIALOG_BOX_PARAM callback function


## -description


<p class="CCE_Message">[The WlxDialogBoxParam function is no longer available for use as of Windows Server 2008 and Windows Vista.]

Called by <a href="https://msdn.microsoft.com/c9567a5b-bd56-4ae1-9eac-af0bb5a6842a">GINA</a> to initialize dialog box controls and then create a modal dialog box from a dialog box template resource.
<div class="alert"><b>Note</b>   GINA DLLs are ignored in Windows Vista.</div><div> </div>

## -parameters




### -param hWlx [in]

Specifies the <a href="https://msdn.microsoft.com/031c898b-3b4d-4b29-811a-112da37b5e3d">Winlogon</a> handle passed to GINA in the 
<a href="https://msdn.microsoft.com/db03f2b3-0719-40be-8a42-04ab7110f711">WlxInitialize</a> call.


### -param hInst [in]

Specifies an instance of the module whose executable file contains the dialog box template.


### -param lpszTemplate [in]

Specifies the dialog box template. This parameter is either the address of a null-terminated character string that specifies the name of the dialog box template, or an integer value that specifies the resource identifier of the dialog box template. If the parameter specifies a resource identifier, its high-order word must be zero and its low-order word must contain the identifier. You can use the 
<a href="https://msdn.microsoft.com/en-us/library/ms648029(v=VS.85).aspx">MAKEINTRESOURCE</a> macro to create this value.


### -param hwndOwner [in]

Specifies the window that owns the dialog box.


### -param dlgprc [in]

Points to the dialog box procedure. For more information about the dialog box procedure, see 
<a href="https://msdn.microsoft.com/library/ms645469(v=VS.85).aspx">DialogProc</a>.


### -param dwInitParam [in]

Specifies the value to pass to the dialog box in the <i>lParam</i> parameter of the 
<a href="https://msdn.microsoft.com/en-us/library/ms645428(v=VS.85).aspx">WM_INITDIALOG</a> message.


## -returns



If the <b>WlxDialogBoxParam</b> function succeeds, the return value is the value of the <i>nResult</i> parameter given in the call to the 
<a href="https://msdn.microsoft.com/en-us/library/ms645472(v=VS.85).aspx">EndDialog</a> function used to terminate the dialog box. The following table lists some possible success return values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WLX_DLG_INPUT_TIMEOUT</b></dt>
</dl>
</td>
<td width="60%">
Input timed out.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WLX_DLG_SAS</b></dt>
</dl>
</td>
<td width="60%">
A <a href="https://msdn.microsoft.com/3e9d7672-2314-45c8-8178-5a0afcfd0c50">secure attention sequence</a> (SAS) event occurred.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WLX_DLG_SCREEN_SAVER_TIMEOUT</b></dt>
</dl>
</td>
<td width="60%">
The screen saver timed out.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WLX_DLG_USER_LOGOFF</b></dt>
</dl>
</td>
<td width="60%">
The user logged off.

</td>
</tr>
</table>
 

If the function fails, the return value is –1.




## -remarks



<b>WlxDialogBoxParam</b> duplicates the Windows <a href="https://msdn.microsoft.com/en-us/library/ms645465(v=VS.85).aspx">DialogBoxParam</a> function, and also allows Winlogon to terminate the dialog box. For more information, see 
<b>DialogBoxParam</b>.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms645465(v=VS.85).aspx">DialogBoxParam</a>



<a href="https://msdn.microsoft.com/library/ms645469(v=VS.85).aspx">DialogProc</a>



<a href="https://msdn.microsoft.com/en-us/library/ms645472(v=VS.85).aspx">EndDialog</a>



<a href="https://msdn.microsoft.com/en-us/library/ms648029(v=VS.85).aspx">MAKEINTRESOURCE</a>



<a href="https://msdn.microsoft.com/db03f2b3-0719-40be-8a42-04ab7110f711">WlxInitialize</a>
 

 
