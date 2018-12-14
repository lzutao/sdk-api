---
UID: NF:faxcomex.IFaxAccountOutgoingArchive.get_SizeHigh
title: IFaxAccountOutgoingArchive::get_SizeHigh
author: windows-sdk-content
description: Specifies the high-order 32-bit value of the size (in bytes) of the archive of outbound fax messages for a particular fax account.
old-location: fax\_mfax_faxaccountoutgoingarchive_cpp_mfax_faxaccountoutgoingarchive_sizehigh_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\reference\serviceextendedcom\i\ifaxaccountoutgoingarchive\sizehigh.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxAccountOutgoingArchive interface [Fax Service],SizeHigh property, IFaxAccountOutgoingArchive.SizeHigh, IFaxAccountOutgoingArchive.get_SizeHigh, IFaxAccountOutgoingArchive::SizeHigh, IFaxAccountOutgoingArchive::get_SizeHigh, SizeHigh property [Fax Service], SizeHigh property [Fax Service],IFaxAccountOutgoingArchive interface, _mfax_faxaccountoutgoingarchive.sizehigh, fax._mfax_faxaccountoutgoingarchive_cpp_mfax_faxaccountoutgoingarchive_sizehigh_cpp, fax._mfax_faxaccountoutgoingarchive_sizehigh, faxcomex/IFaxAccountOutgoingArchive::SizeHigh, faxcomex/IFaxAccountOutgoingArchive::get_SizeHigh, get_SizeHigh
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
 - IFaxAccountOutgoingArchive.SizeHigh
 - IFaxAccountOutgoingArchive.get_SizeHigh
 - IFaxAccountOutgoingArchive.get_SizeHigh
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxAccountOutgoingArchive::get_SizeHigh


## -description


Specifies the high-order 32-bit value of the size (in bytes) of the archive of outbound fax messages for a particular fax account.

This property is read-only.


## -parameters


## -remarks



Because the archive size can exceed 4 GB in size, its size is described as a 64-bit integer whose value is returned as two 32-bit integer values. SizeLow returns the low-order 32-bit value of the archive size. SizeHigh returns the high-order 32-bit value of the archive size. The 64-bit value of the archive size can be computed as: Size64 = (SizeHigh &lt;&lt; 32) + SizeLow.

If both the <a href="https://msdn.microsoft.com/en-us/library/Aa359030(v=VS.85).aspx">SizeLow</a> and <b>SizeHigh</b> properties have the value 0xffffffff, they specify an invalid archive size, and you should ignore both property values.

The property is read-only.

To read this property, a user must have the <a href="https://msdn.microsoft.com/en-us/library/Aa359062(v=VS.85).aspx">far2QUERY_CONFIG</a> access right.




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Aa358948(v=VS.85).aspx">FaxAccountOutgoingArchive</a>



<a href="https://msdn.microsoft.com/en-us/library/Aa359025(v=VS.85).aspx">IFaxAccountOutgoingArchive</a>
 

 
