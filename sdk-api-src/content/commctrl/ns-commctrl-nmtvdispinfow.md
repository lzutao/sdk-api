---
UID: NS:commctrl.tagTVDISPINFOW
title: NMTVDISPINFOW
author: windows-sdk-content
description: Contains and receives display information for a tree-view item. This structure is identical to the TV_DISPINFO structure, but it has been renamed to follow current naming conventions.
old-location: controls\NMTVDISPINFO.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\treeview\structures\nmtvdispinfo.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPNMTVDISPINFOW, LPNMTVDISPINFO, LPNMTVDISPINFO structure pointer [Windows Controls], NMTVDISPINFO, NMTVDISPINFO structure [Windows Controls], NMTVDISPINFOA, NMTVDISPINFOW, TVIF_CHILDREN, TVIF_IMAGE, TVIF_SELECTEDIMAGE, TVIF_TEXT, _win32_NMTVDISPINFO, _win32_NMTVDISPINFO_cpp, commctrl/LPNMTVDISPINFO, commctrl/NMTVDISPINFO, commctrl/NMTVDISPINFOA, commctrl/NMTVDISPINFOW, controls.NMTVDISPINFO, controls._win32_NMTVDISPINFO"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: NMTVDISPINFOW (Unicode) and NMTVDISPINFOA (ANSI)
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
 - Commctrl.h
api_name:
 - NMTVDISPINFO
 - NMTVDISPINFOA
 - NMTVDISPINFOW
product: Windows
targetos: Windows
req.typenames: NMTVDISPINFOW, *LPNMTVDISPINFOW
req.redist: 
---

# NMTVDISPINFOW structure


## -description


Contains and receives display information for a tree-view item. This structure is identical to the 
			<b>TV_DISPINFO</b> structure, but it has been renamed to follow current naming conventions. 


## -struct-fields




### -field hdr

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb775514(v=VS.85).aspx">NMHDR</a> structure that contains information about this notification. 


### -field item

Type: <b><a href="https://msdn.microsoft.com/en-us/library/Bb773456(v=VS.85).aspx">TVITEM</a></b>


<a href="https://msdn.microsoft.com/en-us/library/Bb773456(v=VS.85).aspx">TVITEM</a> structure that identifies and contains information about the tree-view item. The 
					<b>mask</b> member of the <b>TVITEM</b> structure specifies which information is being set or retrieved. It can be one or more of the following values: 

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="TVIF_CHILDREN"></a><a id="tvif_children"></a><dl>
<dt><b>TVIF_CHILDREN</b></dt>
</dl>
</td>
<td width="60%">
The 
						<b>cChildren</b> member specifies, or is to receive, a value that indicates whether the item has child items. 

</td>
</tr>
<tr>
<td width="40%"><a id="TVIF_IMAGE"></a><a id="tvif_image"></a><dl>
<dt><b>TVIF_IMAGE</b></dt>
</dl>
</td>
<td width="60%">
The 
						<b>iImage</b> member specifies, or is to receive, the index of the item's nonselected icon in the image list. 

</td>
</tr>
<tr>
<td width="40%"><a id="TVIF_SELECTEDIMAGE"></a><a id="tvif_selectedimage"></a><dl>
<dt><b>TVIF_SELECTEDIMAGE</b></dt>
</dl>
</td>
<td width="60%">
The 
						<b>iSelectedImage</b> member specifies, or is to receive, the index of the item's selected icon in the image list. 

</td>
</tr>
<tr>
<td width="40%"><a id="TVIF_TEXT"></a><a id="tvif_text"></a><dl>
<dt><b>TVIF_TEXT</b></dt>
</dl>
</td>
<td width="60%">
The 
						<b>pszText</b> member specifies the new item text or the address of a buffer that is to receive the item text. If the structure is receiving item text, you typically copy the text to the buffer pointed to by the 
						<b>pszText</b> member of the <a href="https://msdn.microsoft.com/en-us/library/Bb773456(v=VS.85).aspx">TVITEM</a> structure. However, you can return a string in the 
						<b>pszText</b> member instead. If you do so, you cannot change or delete the string until the corresponding item text is deleted or until two additional <a href="https://msdn.microsoft.com/en-us/library/Bb773518(v=VS.85).aspx">TVN_GETDISPINFO</a> notification codes have been sent. 

</td>
</tr>
</table>
 


## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/en-us/library/Bb773551(v=VS.85).aspx">TVN_SETDISPINFO</a>



<a href="https://msdn.microsoft.com/en-us/library/Bb775583(v=VS.85).aspx">WM_NOTIFY</a>
 

 
