---
UID: NF:faxcomex.IFaxAccountSet.RemoveAccount
title: IFaxAccountSet::RemoveAccount
author: windows-sdk-content
description: Removes a fax account from the fax server.
old-location: fax\_mfax_faxaccountset_cpp_mfax_faxaccountset_removeaccount_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\reference\serviceextendedcom\i\ifaxaccountset\removeaccount.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxAccountSet interface [Fax Service],RemoveAccount method, IFaxAccountSet.RemoveAccount, IFaxAccountSet::RemoveAccount, RemoveAccount, RemoveAccount method [Fax Service], RemoveAccount method [Fax Service],IFaxAccountSet interface, _mfax_faxaccountset.removeaccount, fax._mfax_faxaccountset_cpp_mfax_faxaccountset_removeaccount_cpp, fax._mfax_faxaccountset_removeaccount, faxcomex/IFaxAccountSet::RemoveAccount
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcomex.h
req.include-header: 
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
req.lib: 
req.dll: Fxscomex.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Fxscomex.dll
api_name:
 - IFaxAccountSet.RemoveAccount
 - IFaxAccountSet.RemoveAccount
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxAccountSet::RemoveAccount


## -description


Removes a fax account from the fax server.


## -parameters




### -param bstrAccountName [in]

Type: <b>BSTR</b>

Specifies a null-terminated string that contains the name of the account to be removed.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



<i>bstrAccountName</i> must be of the form &lt;domainName&gt;\&lt;username&gt; or just &lt;username&gt; for local users.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa358935(v=VS.85).aspx">FaxAccountSet</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa359014(v=VS.85).aspx">IFaxAccountSet</a>
 

 
