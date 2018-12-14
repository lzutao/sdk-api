---
UID: NS:ws2ipdef.sockaddr_in6
title: SOCKADDR_IN6_LH
author: windows-sdk-content
description: The SOCKADDR_IN6 structure specifies a transport address and port for the AF_INET6 address family.
old-location: netvista\sockaddr_in6.htm
tech.root: NetVista
ms.assetid: ef2955d2-5dc1-420b-a9e0-32a584059d5a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*LPSOCKADDR_IN6, *LPSOCKADDR_IN6_LH, *PSOCKADDR_IN6, *PSOCKADDR_IN6_LH, PSOCKADDR_IN6, PSOCKADDR_IN6 structure pointer [Network Drivers Starting with Windows Vista], SOCKADDR_IN6, SOCKADDR_IN6 structure [Network Drivers Starting with Windows Vista], SOCKADDR_IN6_LH, netvista.sockaddr_in6, ws2ipdef/PSOCKADDR_IN6, ws2ipdef/SOCKADDR_IN6, wskref_7e70684f-ef0d-45c5-8075-3e9b6fa87337.xml"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ws2ipdef.h
req.include-header: Ws2ipdef.h
req.target-type: Windows
req.target-min-winverclnt: Available in Windows Vista and later versions of the Windows operating   systems.
req.target-min-winversvr: 
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
 - Ws2ipdef.h
api_name:
 - SOCKADDR_IN6
product: Windows
targetos: Windows
req.typenames: SOCKADDR_IN6_LH, *PSOCKADDR_IN6_LH, *LPSOCKADDR_IN6_LH
req.redist: 
---

# SOCKADDR_IN6_LH structure


## -description


The SOCKADDR_IN6 structure specifies a transport address and port for the 
  <a href="netvista.af_inet6">AF_INET6</a> address family.


## -struct-fields




### -field sin6_family

The address family for the transport address. This member should always be set to AF_INET6.


### -field sin6_port

A transport protocol port number.


### -field sin6_flowinfo

The IPv6 flow information.


### -field sin6_addr

An 
     <a href="https://msdn.microsoft.com/218b07e8-94cf-42f2-a762-13fc1f7c4473">IN6_ADDR</a> structure that contains an IPv6 transport
     address.


### -field sin6_scope_id

A ULONG representation of the IPv6 scope identifier that is defined in the 
      <b>sin6_scope_struct</b> member.


### -field sin6_scope_struct

A SCOPE_ID structure that contains the scope identifier for the IPv6 transport address. The
      SCOPE_ID structure is defined as follows:
      

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>typedef struct {
  union {
    struct {
      ULONG  Zone : 28;
      ULONG  Level : 4;
    };
    ULONG  Value;
  };
} SCOPE_ID, *PSCOPE_ID;</pre>
</td>
</tr>
</table></span></div>




#### Zone

The zone index that identifies the zone to which the transport address pertains. Zones of the
        different scopes are instantiated as follows:
        

<ul>
<li>Each interface on a node comprises a single zone of interface-local scope.</li>
</ul>
<ul>
<li>Each link, and the interfaces attached to that link, comprise a single zone of link-local
         scope.</li>
</ul>
<ul>
<li>There is a single zone of global scope that comprises all of the links and interfaces in the
         Internet.</li>
</ul>
<ul>
<li>The boundaries of zones of scope other than interface-local, link-local, and global are
         defined by network administrators.</li>
</ul>
A value of zero specifies the default zone.



#### Level

The scope of the IPv6 transport address. This scope must be the same as the IPv6 scope value
        that is embedded in the IPv6 transport address. This member can be one of the following:
        

<b>ScopeLevelInterface</b>

The transport address has interface-local scope.

<b>ScopeLevelLink</b>

The transport address has link-local scope.

<b>ScopeLevelSubnet</b>

The transport address has subnet-local scope.

<b>ScopeLevelAdmin</b>

The transport address has admin-local scope.

<b>ScopeLevelSite</b>

The transport address has site-local scope.

<b>ScopeLevelOrganization</b>

The transport address has organization-local scope.

<b>ScopeLevelGlobal</b>

The transport address has global scope.



#### Value

A ULONG representation of the IPv6 scope identifier.


## -remarks



All of the data in the SOCKADDR_IN6 structure, except for the address family, must be specified in
    network-byte-order (big-endian).

The size of the SOCKADDR_IN6 structure is too large to fit in the memory space that is provided by a 
    <a href="https://msdn.microsoft.com/af5ad9ae-3987-4f16-a8a6-14e3e3d0fa6a">SOCKADDR</a> structure. For a structure that is
    guaranteed to be large enough to contain a transport address for all possible address families, see 
    <a href="https://msdn.microsoft.com/27e56c1a-ce11-4cdb-9be8-25ed2f94fb37">SOCKADDR_STORAGE</a>.




## -see-also




<a href="netvista.af_inet6">AF_INET6</a>



<a href="https://msdn.microsoft.com/218b07e8-94cf-42f2-a762-13fc1f7c4473">IN6_ADDR</a>



<a href="https://msdn.microsoft.com/af5ad9ae-3987-4f16-a8a6-14e3e3d0fa6a">SOCKADDR</a>



<a href="https://msdn.microsoft.com/27e56c1a-ce11-4cdb-9be8-25ed2f94fb37">SOCKADDR_STORAGE</a>
 

 
