---
UID: NF:faxcomex.IFaxOutboundRoutingRules.RemoveByCountryAndArea
title: IFaxOutboundRoutingRules::RemoveByCountryAndArea
author: windows-sdk-content
description: The IFaxOutboundRoutingRules::RemoveByCountryAndArea method removes an outbound routing rule (FaxOutboundRoutingRule object) from the collection using the routing rule's country/region code and area code.
old-location: fax\_mfax_faxoutboundroutingrules_cpp_mfax_faxoutboundroutingrules_removebycountryandarea_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinto_z_62e9.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IFaxOutboundRoutingRules interface [Fax Service],RemoveByCountryAndArea method, IFaxOutboundRoutingRules.RemoveByCountryAndArea, IFaxOutboundRoutingRules::RemoveByCountryAndArea, RemoveByCountryAndArea, RemoveByCountryAndArea method [Fax Service], RemoveByCountryAndArea method [Fax Service],IFaxOutboundRoutingRules interface, _mfax_faxoutboundroutingrules.removebycountryandarea, fax._mfax_faxoutboundroutingrules_cpp_mfax_faxoutboundroutingrules_removebycountryandarea_cpp, fax._mfax_faxoutboundroutingrules_removebycountryandarea, faxcomex/IFaxOutboundRoutingRules::RemoveByCountryAndArea
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: faxcomex.h
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
 - IFaxOutboundRoutingRules.RemoveByCountryAndArea
 - IFaxOutboundRoutingRules.RemoveByCountryAndArea
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IFaxOutboundRoutingRules::RemoveByCountryAndArea


## -description


The <b>IFaxOutboundRoutingRules::RemoveByCountryAndArea</b> method removes an outbound routing rule (<a href="https://msdn.microsoft.com/en-us/library/ms690230(v=VS.85).aspx">FaxOutboundRoutingRule</a> object) from the collection using the routing rule's country/region code and area code.


## -parameters




### -param lCountryCode

Type: <b>long</b>

A <b>long</b> value that specifies the country/region code of the outbound routing rule to remove from the collection. Specifying <a href="https://msdn.microsoft.com/en-us/library/ms687973(v=VS.85).aspx">frrcANY_CODE</a> will remove a rule that applies to all country/region codes.


### -param lAreaCode

Type: <b>long</b>

A <b>long</b> value that specifies the area code of the outbound routing rule to remove from the collection. Specifying <a href="https://msdn.microsoft.com/en-us/library/ms687973(v=VS.85).aspx">frrcANY_CODE</a> will remove a rule that applies to all area codes within the specified country/region code.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



You cannot set both <i>lCountryCode</i> and <i>lAreaCode</i> to <a href="https://msdn.microsoft.com/en-us/library/ms687973(v=VS.85).aspx">frrcANY_CODE</a> because this is equivalent to specifying the default outbound routing rule, which cannot be removed. 




## -see-also




<a href="https://msdn.microsoft.com/en-us/library/ms689525(v=VS.85).aspx">FaxOutboundRoutingRules</a>



<a href="https://msdn.microsoft.com/en-us/library/ms689527(v=VS.85).aspx">IFaxOutboundRoutingRules</a>



<a href="https://msdn.microsoft.com/en-us/library/ms693486(v=VS.85).aspx">Visual Basic Example</a>
 

 
