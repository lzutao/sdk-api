---
UID: NE:structuredquery.tagSTRUCTURED_QUERY_MULTIOPTION
title: STRUCTURED_QUERY_MULTIOPTION
author: windows-sdk-content
description: A set of flags used by IQueryParser::SetMultiOption to indicate individual options.
old-location: search\_search_STRUCTURED_QUERY_MULTIOPTION.htm
tech.root: search
ms.assetid: VS|search|~\search\wds3x\reference\enums\structured_query_multioption.htm
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: SQMO_DEFAULT_PROPERTY, SQMO_GENERATOR_FOR_TYPE, SQMO_MAP_PROPERTY, SQMO_VIRTUAL_PROPERTY, STRUCTURED_QUERY_MULTIOPTION, STRUCTURED_QUERY_MULTIOPTION enumeration [search], _search_STRUCTURED_QUERY_MULTIOPTION, search._search_STRUCTURED_QUERY_MULTIOPTION, structuredquery/SQMO_DEFAULT_PROPERTY, structuredquery/SQMO_GENERATOR_FOR_TYPE, structuredquery/SQMO_MAP_PROPERTY, structuredquery/SQMO_VIRTUAL_PROPERTY, structuredquery/STRUCTURED_QUERY_MULTIOPTION
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: structuredquery.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Structuredquery.idl
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
 - Structuredquery.h
api_name:
 - STRUCTURED_QUERY_MULTIOPTION
product: Windows
targetos: Windows
req.typenames: STRUCTURED_QUERY_MULTIOPTION
req.redist: Windows Desktop Search (WDS) 3.0
---

# STRUCTURED_QUERY_MULTIOPTION enumeration


## -description


A set of flags used by <a href="https://msdn.microsoft.com/en-us/library/Bb231358(v=VS.85).aspx">IQueryParser::SetMultiOption</a> to indicate individual options.


## -enum-fields




### -field SQMO_VIRTUAL_PROPERTY

To indicate that a leaf node with property name P and constant C should be replaced with a leaf node with property name Q, operation op, and constant C by <a href="https://msdn.microsoft.com/en-us/library/Bb231387(v=VS.85).aspx">IConditionFactory::Resolve</a>, do the following: call <a href="https://msdn.microsoft.com/en-us/library/Bb231358(v=VS.85).aspx">IQueryParser::SetMultiOption</a> with SQMO_VIRTUAL_PROPERTY as <i>option</i>, P as <i>pszOptionKey</i>, and for <i>pOptionValue</i> provide a <b>VT_UNKNOWN</b> with an <a href="https://msdn.microsoft.com/en-us/library/ms221053(v=VS.85).aspx">IEnumVARIANT</a> interface that enumerates exactly two values: a <b>VT_BSTR</b> with value Q, and a <b>VT_I4</b> that is a <a href="https://msdn.microsoft.com/en-us/library/Aa965691(v=VS.85).aspx">CONDITION_OPERATION</a> operation.


### -field SQMO_DEFAULT_PROPERTY

To indicate that a leaf node with no property name and a semantic type T (or one that is a subtype of T) should be replaced with one having property name P by <a href="https://msdn.microsoft.com/en-us/library/Bb231387(v=VS.85).aspx">IConditionFactory::Resolve</a>, do the following: call <a href="https://msdn.microsoft.com/en-us/library/Bb231358(v=VS.85).aspx">IQueryParser::SetMultiOption</a> with SQMO_DEFAULT_PROPERTY  as <i>option</i>, T as <i>pszOptionKey</i>, and for <i>pOptionValue</i> provide a <b>VT_LPWSTR</b> with value P.


### -field SQMO_GENERATOR_FOR_TYPE

To indicate that an <a href="https://msdn.microsoft.com/en-us/library/Bb231380(v=VS.85).aspx">IConditionGenerator</a> G should be used to recognize named entities of the semantic type named T, and that <a href="https://msdn.microsoft.com/en-us/library/Bb231387(v=VS.85).aspx">IConditionFactory::Resolve</a> should generate condition trees for those named entities, call <a href="https://msdn.microsoft.com/en-us/library/Bb231358(v=VS.85).aspx">IQueryParser::SetMultiOption</a> with SQMO_GENERATOR_FOR_TYPE as <i>option</i>, T as <i>pszOptionKey</i> and for <i>pOptionValue</i> provide a <b>VT_UNKNOWN</b> with value G.


### -field SQMO_MAP_PROPERTY

Windows 7, and later. To indicate that a node with property P should map to one or more other properties, call <a href="https://msdn.microsoft.com/en-us/library/Bb231358(v=VS.85).aspx">IQueryParser::SetMultiOption</a> with SQMO_MAP_PROPERTY as <i>option</i>, P as <i>pszOptionKey</i>, and for <i>pOptionValue</i> provide a <b>VT_VECTOR</b> or <b>VT_LPWSTR</b>, where each string is a property name. During resolustion, this map is added to those of the loaded schema. Calling <b>IQueryParser::SetMultiOption</b> with <i>pOptionValue</i> as <b>VT_NULL</b> removes the mapping.
