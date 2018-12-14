---
UID: NE:shldisp._tagAUTOCOMPLETEOPTIONS
title: AUTOCOMPLETEOPTIONS
author: windows-sdk-content
description: Specifies values used by IAutoComplete2::GetOptions and IAutoComplete2::SetOptions for options surrounding autocomplete.
old-location: shell\AUTOCOMPLETEOPTIONS.htm
tech.root: shell
ms.assetid: e0a583da-c2bd-4757-868d-a63e697142e2
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: ACO_AUTOAPPEND, ACO_AUTOSUGGEST, ACO_FILTERPREFIXES, ACO_NONE, ACO_NOPREFIXFILTERING, ACO_RTLREADING, ACO_SEARCH, ACO_UPDOWNKEYDROPSLIST, ACO_USETAB, ACO_WORD_FILTER, AUTOCOMPLETEOPTIONS, AUTOCOMPLETEOPTIONS enumeration [Windows Shell], _shell_AUTOCOMPLETEOPTIONS, shell.AUTOCOMPLETEOPTIONS, shldisp/ACO_AUTOAPPEND, shldisp/ACO_AUTOSUGGEST, shldisp/ACO_FILTERPREFIXES, shldisp/ACO_NONE, shldisp/ACO_NOPREFIXFILTERING, shldisp/ACO_RTLREADING, shldisp/ACO_SEARCH, shldisp/ACO_UPDOWNKEYDROPSLIST, shldisp/ACO_USETAB, shldisp/ACO_WORD_FILTER, shldisp/AUTOCOMPLETEOPTIONS
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: shldisp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional with SP3 [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shldisp.idl
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
 - Shldisp.h
api_name:
 - AUTOCOMPLETEOPTIONS
product: Windows
targetos: Windows
req.typenames: AUTOCOMPLETEOPTIONS
req.redist: 
---

# AUTOCOMPLETEOPTIONS enumeration


## -description


Specifies values used by <a href="https://msdn.microsoft.com/00c2aa5f-eebc-479c-ac33-6efb3acb1051">IAutoComplete2::GetOptions</a> and <a href="https://msdn.microsoft.com/d3562845-fc28-4726-a520-29720f9924fc">IAutoComplete2::SetOptions</a> for options surrounding autocomplete.


## -enum-fields




### -field ACO_NONE

0x0000. Do not autocomplete.


### -field ACO_AUTOSUGGEST

0x0001. Enable the autosuggest drop-down list.


### -field ACO_AUTOAPPEND

0x0002. Enable autoappend.


### -field ACO_SEARCH

0x0004. Add a search item to the list of completed strings. When the user selects this item, it launches a search engine.


### -field ACO_FILTERPREFIXES

0x0008. Do not match common prefixes, such as "www." or "http://".


### -field ACO_USETAB

0x0010. Use the TAB key to select an item from the drop-down list.


### -field ACO_UPDOWNKEYDROPSLIST

0x0020. Use the UP ARROW and DOWN ARROW keys to display the autosuggest drop-down list.


### -field ACO_RTLREADING

0x0040. Normal windows display text left-to-right (LTR). Windows can be mirrored to display languages such as Hebrew or Arabic that read right-to-left (RTL). Typically, control text is displayed in the same direction as the text in its parent window. If <a href="https://msdn.microsoft.com/e0a583da-c2bd-4757-868d-a63e697142e2">ACO_RTLREADING</a> is set, the text reads in the opposite direction from the text in the parent window.


### -field ACO_WORD_FILTER

0x0080. <b>Windows Vista and later</b>. If set, the autocompleted suggestion is treated as a phrase for search purposes. The suggestion, <i>Microsoft Office</i>, would be treated as <i>"Microsoft Office"</i> (where both <i>Microsoft</i> AND <i>Office</i> must appear in the search results).


### -field ACO_NOPREFIXFILTERING

0x0100. <b>Windows Vista and later</b>. Disable prefix filtering when displaying the autosuggest dropdown. Always display all suggestions.
