---
UID: NC:ddeml.PFNCALLBACK
title: PFNCALLBACK
author: windows-sdk-content
description: An application-defined callback function used with the Dynamic Data Exchange Management Library (DDEML) functions.
old-location: dataxchg\ddecallback.htm
tech.root: dataxchg
ms.assetid: VS|winui|~\winui\windowsuserinterface\dataexchange\dynamicdataexchangemanagementlibrary\dynamicdataexchangemanagementreference\dynamicdataexchangemanagementfunctions\ddecallback.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: PFNCALLBACK, PFNCALLBACK callback, PFNCALLBACK callback function [Data Exchange], XCLASS_BOOL, XCLASS_DATA, XCLASS_FLAGS, XCLASS_NOTIFICATION, _win32_DdeCallback, _win32_ddecallback_cpp, dataxchg.ddecallback, ddeml/PFNCALLBACK, winui._win32_ddecallback
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: ddeml.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
 - Ddeml.h
api_name:
 - PFNCALLBACK
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# PFNCALLBACK callback function


## -description


An application-defined callback function used with the <a href="https://msdn.microsoft.com/en-us/library/ms648712(v=VS.85).aspx">Dynamic Data Exchange Management Library</a> (DDEML) functions. It processes Dynamic Data Exchange (DDE) transactions. The 
			<b>PFNCALLBACK</b> type defines a pointer to this callback function. <i>DdeCallback</i> is a placeholder for the application-defined function name. 


## -parameters




### -param wType


### -param wFmt


### -param hConv


### -param hsz1 [in]

Type: <b>HSZ</b>

A handle to a string. The meaning of this parameter depends on the type of the current transaction. For the meaning of this parameter, see the description of the transaction type. 


### -param hsz2 [in]

Type: <b>HSZ</b>

A handle to a string. The meaning of this parameter depends on the type of the current transaction. For the meaning of this parameter, see the description of the transaction type. 


### -param hData


### -param dwData1 [in]

Type: <b>ULONG_PTR</b>

Transaction-specific data. For the meaning of this parameter, see the description of the transaction type. 


### -param dwData2 [in]

Type: <b>ULONG_PTR</b>

Transaction-specific data. For the meaning of this parameter, see the description of the transaction type. 


#### - hconv [in]

Type: <b>HCONV</b>

A handle to the conversation associated with the current transaction. 


#### - hdata [in]

Type: <b>HDDEDATA</b>

A handle to DDE data. The meaning of this parameter depends on the type of the current transaction. For the meaning of this parameter, see the description of the transaction type. 


#### - uFmt [in]

Type: <b>UINT</b>

The format in which data is sent or received. 


#### - uType [in]

Type: <b>UINT</b>

The type of the current transaction. This parameter consists of a combination of transaction class flags and transaction type flags. The following table describes each of the transaction classes and provides a list of the transaction types in each class. For information about a specific transaction type, see the individual description of that type. 



#### XCLASS_BOOL

A DDE callback function should return <b>TRUE</b> or <b>FALSE</b> when it finishes processing a transaction that belongs to this class. The <b>XCLASS_BOOL</b> transaction class consists of the following types: 
                        

<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648716(v=VS.85).aspx">XTYP_ADVSTART</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648718(v=VS.85).aspx">XTYP_CONNECT</a>
</li>
</ul>


#### XCLASS_DATA

A DDE callback function should return a DDE handle, the <b>CBR_BLOCK</b> return code, or <b>NULL</b> when it finishes processing a transaction that belongs to this class. The <b>XCLASS_DATA</b> transaction class consists of the following types: 
                        

<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648715(v=VS.85).aspx">XTYP_ADVREQ</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648726(v=VS.85).aspx">XTYP_REQUEST</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648728(v=VS.85).aspx">XTYP_WILDCONNECT</a>
</li>
</ul>


#### XCLASS_FLAGS

A DDE callback function should return <b>DDE_FACK</b>, <b>DDE_FBUSY</b>, or <b>DDE_FNOTPROCESSED</b> when it finishes processing a transaction that belongs to this class. The <b>XCLASS_FLAGS</b> transaction class consists of the following types:
                        

<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648714(v=VS.85).aspx">XTYP_ADVDATA</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648722(v=VS.85).aspx">XTYP_EXECUTE</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648724(v=VS.85).aspx">XTYP_POKE</a>
</li>
</ul>


#### XCLASS_NOTIFICATION

The transaction types that belong to this class are for notification purposes only. The return value from the callback function is ignored. The <b>XCLASS_NOTIFICATION</b> transaction class consists of the following types: 
						

<ul>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648717(v=VS.85).aspx">XTYP_ADVSTOP</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648719(v=VS.85).aspx">XTYP_CONNECT_CONFIRM</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648720(v=VS.85).aspx">XTYP_DISCONNECT</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648721(v=VS.85).aspx">XTYP_ERROR</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648723(v=VS.85).aspx">XTYP_MONITOR</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648725(v=VS.85).aspx">XTYP_REGISTER</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648729(v=VS.85).aspx">XTYP_XACT_COMPLETE</a>
</li>
<li>
<a href="https://msdn.microsoft.com/en-us/library/ms648727(v=VS.85).aspx">XTYP_UNREGISTER</a>
</li>
</ul>

## -returns



Type: <b>HDDEDATA</b>

The return value depends on the transaction class. For more information about the return values, see descriptions of the individual transaction types. 




## -remarks



The callback function is called asynchronously for transactions that do not involve the creation or termination of conversations. An application that does not frequently accept incoming messages will have reduced DDE performance because the Dynamic Data Exchange Management Library (DDEML) uses messages to initiate transactions. 

An application must register the callback function by specifying a pointer to the function in a call to the <a href="https://msdn.microsoft.com/en-us/library/ms648757(v=VS.85).aspx">DdeInitialize</a> function. 




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/en-us/library/ms648751(v=VS.85).aspx">DdeEnableCallback</a>



<a href="https://msdn.microsoft.com/en-us/library/ms648757(v=VS.85).aspx">DdeInitialize</a>



<a href="https://msdn.microsoft.com/en-us/library/ms648712(v=VS.85).aspx">Dynamic Data Exchange Management Library</a>



<b>Reference</b>
 

 
