---
UID: NE:dsrole._DSROLE_MACHINE_ROLE
title: DSROLE_MACHINE_ROLE
author: windows-sdk-content
description: Used with the MachineRole member of the DSROLE_PRIMARY_DOMAIN_INFO_BASIC structure to specify the computer role.
old-location: ad\dsrole_machine_role.htm
tech.root: ad
ms.assetid: d5255070-71dd-4510-8bec-a84726a241c6
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: DSROLE_MACHINE_ROLE, DSROLE_MACHINE_ROLE enumeration [Active Directory], DsRole_RoleBackupDomainController, DsRole_RoleMemberServer, DsRole_RoleMemberWorkstation, DsRole_RolePrimaryDomainController, DsRole_RoleStandaloneServer, DsRole_RoleStandaloneWorkstation, ad.dsrole_machine_role, dsrole/DSROLE_MACHINE_ROLE, dsrole/DsRole_RoleBackupDomainController, dsrole/DsRole_RoleMemberServer, dsrole/DsRole_RoleMemberWorkstation, dsrole/DsRole_RolePrimaryDomainController, dsrole/DsRole_RoleStandaloneServer, dsrole/DsRole_RoleStandaloneWorkstation
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: dsrole.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
 - Dsrole.h
api_name:
 - DSROLE_MACHINE_ROLE
product: Windows
targetos: Windows
req.typenames: DSROLE_MACHINE_ROLE
req.redist: 
---

# DSROLE_MACHINE_ROLE enumeration


## -description


The <b>DSROLE_MACHINE_ROLE</b> enumeration is used with the <b>MachineRole</b> member of the <a href="https://msdn.microsoft.com/8a7b34e8-46d6-46dc-9fef-ec37b0f65eea">DSROLE_PRIMARY_DOMAIN_INFO_BASIC</a> structure to specify the computer role.


## -enum-fields




### -field DsRole_RoleStandaloneWorkstation

The computer is a workstation that is not a member of a domain.


### -field DsRole_RoleMemberWorkstation

The computer is a workstation that is a member of a domain.


### -field DsRole_RoleStandaloneServer

The computer is a server that is not a member of a domain.


### -field DsRole_RoleMemberServer

The computer is a server that is a member of a domain.


### -field DsRole_RoleBackupDomainController

The computer is a backup domain controller.


### -field DsRole_RolePrimaryDomainController

The computer is a primary domain controller.


## -see-also




<a href="https://msdn.microsoft.com/8a7b34e8-46d6-46dc-9fef-ec37b0f65eea">DSROLE_PRIMARY_DOMAIN_INFO_BASIC</a>



<a href="https://msdn.microsoft.com/eafa3285-4474-4077-a6ad-b37f8211e7e6">Enumerations in Active Directory Domain Services</a>
 

 
