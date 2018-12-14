---
UID: NE:ndattrib.__MIDL___MIDL_itf_ndattrib_0000_0000_0002
title: REPAIR_RISK
author: windows-sdk-content
description: The REPAIR_RISK enumeration specifies whether repair changes are persistent and whether they can be undone.
old-location: ndf\repair_risk.htm
tech.root: NDF
ms.assetid: 016e047e-9962-4b27-bd5d-8dd6b826ae03
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: REPAIR_RISK, REPAIR_RISK enumeration [NDF], RR_NORISK, RR_NOROLLBACK, RR_ROLLBACK, ndattrib/REPAIR_RISK, ndattrib/RR_NORISK, ndattrib/RR_NOROLLBACK, ndattrib/RR_ROLLBACK, ndf.repair_risk
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: ndattrib.h
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
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Ndattrib.h
api_name:
 - REPAIR_RISK
product: Windows
targetos: Windows
req.typenames: REPAIR_RISK
req.redist: 
---

# REPAIR_RISK enumeration


## -description


The <b>REPAIR_RISK</b> enumeration specifies whether repair changes are persistent and whether they can be undone.


## -enum-fields




### -field RR_NOROLLBACK

The repair performs persistent changes that cannot be undone.


### -field RR_ROLLBACK

The repair performs persistent changes that can be undone.


### -field RR_NORISK

The repair does not perform persistent changes.
