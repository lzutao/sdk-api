---
UID: NS:vds._VDS_POOL_ATTRIBUTES
title: VDS_POOL_ATTRIBUTES
author: windows-sdk-content
description: Defines the attributes of a storage pool.
old-location: base\vds_pool_attributes.htm
tech.root: vds
ms.assetid: 3dfbd3d9-ec2e-44ac-9d0f-7aa6c530db18
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PVDS_POOL_ATTRIBUTES, PVDS_POOL_ATTRIBUTES, PVDS_POOL_ATTRIBUTES structure pointer, VDS_POOL_ATTRIBUTES, VDS_POOL_ATTRIBUTES structure, VDS_POOL_ATTRIB_ACCS_BDW_WT_HINT, VDS_POOL_ATTRIB_ACCS_DIR_HINT, VDS_POOL_ATTRIB_ACCS_LTNCY_HINT, VDS_POOL_ATTRIB_ACCS_RNDM_HINT, VDS_POOL_ATTRIB_ACCS_SIZE_HINT, VDS_POOL_ATTRIB_ALLOW_SPINDOWN, VDS_POOL_ATTRIB_BUSTYPE, VDS_POOL_ATTRIB_CUSTOM_ATTRIB, VDS_POOL_ATTRIB_DATA_AVL_HINT, VDS_POOL_ATTRIB_DATA_RDNCY_DEF, VDS_POOL_ATTRIB_DATA_RDNCY_MAX, VDS_POOL_ATTRIB_DATA_RDNCY_MIN, VDS_POOL_ATTRIB_NO_SINGLE_POF, VDS_POOL_ATTRIB_NUM_CLMNS, VDS_POOL_ATTRIB_NUM_CLMNS_DEF, VDS_POOL_ATTRIB_NUM_CLMNS_MAX, VDS_POOL_ATTRIB_NUM_CLMNS_MIN, VDS_POOL_ATTRIB_PKG_RDNCY_DEF, VDS_POOL_ATTRIB_PKG_RDNCY_MAX, VDS_POOL_ATTRIB_PKG_RDNCY_MIN, VDS_POOL_ATTRIB_RAIDTYPE, VDS_POOL_ATTRIB_STOR_COST_HINT, VDS_POOL_ATTRIB_STOR_EFFCY_HINT, VDS_POOL_ATTRIB_STRIPE_SIZE, VDS_POOL_ATTRIB_STRIPE_SIZE_DEF, VDS_POOL_ATTRIB_STRIPE_SIZE_MAX, VDS_POOL_ATTRIB_STRIPE_SIZE_MIN, VDS_POOL_ATTRIB_THIN_PROVISION, base.vds_pool_attributes, vds/PVDS_POOL_ATTRIBUTES, vds/VDS_POOL_ATTRIBUTES, vdshwprv/PVDS_POOL_ATTRIBUTES, vdshwprv/VDS_POOL_ATTRIBUTES"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
 - Vds.h
 - VdsHwPrv.h
api_name:
 - VDS_POOL_ATTRIBUTES
product: Windows
targetos: Windows
req.typenames: VDS_POOL_ATTRIBUTES, *PVDS_POOL_ATTRIBUTES
req.redist: 
---

# VDS_POOL_ATTRIBUTES structure


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Defines the attributes of a <a href="https://msdn.microsoft.com/a6104742-3ef9-4570-9728-3e6580953117">storage pool</a>.


## -struct-fields




### -field ullAttributeMask

A mask that specifies the attributes in the structure that are defined by this storage pool. 


The list of valid attribute flags is as follows. Each flag corresponds to a member in the <b>VDS_POOL_ATTRIBUTES</b> structure. Unused bits are reserved.



<table>
<tr>
<th>Value</th>
<th>Attribute defined by the storage pool</th>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_RAIDTYPE"></a><a id="vds_pool_attrib_raidtype"></a><dl>
<dt><b>VDS_POOL_ATTRIB_RAIDTYPE</b></dt>
<dt>0x1L</dt>
</dl>
</td>
<td width="60%">
<b>raidType</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_BUSTYPE"></a><a id="vds_pool_attrib_bustype"></a><dl>
<dt><b>VDS_POOL_ATTRIB_BUSTYPE</b></dt>
<dt>0x2L</dt>
</dl>
</td>
<td width="60%">
<b>busType</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_ALLOW_SPINDOWN"></a><a id="vds_pool_attrib_allow_spindown"></a><dl>
<dt><b>VDS_POOL_ATTRIB_ALLOW_SPINDOWN</b></dt>
<dt>0x4L</dt>
</dl>
</td>
<td width="60%">
<b>bSpinDown</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_THIN_PROVISION"></a><a id="vds_pool_attrib_thin_provision"></a><dl>
<dt><b>VDS_POOL_ATTRIB_THIN_PROVISION</b></dt>
<dt>0x8L</dt>
</dl>
</td>
<td width="60%">
<b>bIsThinProvisioned</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_NO_SINGLE_POF"></a><a id="vds_pool_attrib_no_single_pof"></a><dl>
<dt><b>VDS_POOL_ATTRIB_NO_SINGLE_POF</b></dt>
<dt>0x10L</dt>
</dl>
</td>
<td width="60%">
<b>bNoSinglePointOfFailure</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_DATA_RDNCY_MAX"></a><a id="vds_pool_attrib_data_rdncy_max"></a><dl>
<dt><b>VDS_POOL_ATTRIB_DATA_RDNCY_MAX</b></dt>
<dt>0x20L</dt>
</dl>
</td>
<td width="60%">
<b>ulDataRedundancyMax</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_DATA_RDNCY_MIN"></a><a id="vds_pool_attrib_data_rdncy_min"></a><dl>
<dt><b>VDS_POOL_ATTRIB_DATA_RDNCY_MIN</b></dt>
<dt>0x40L</dt>
</dl>
</td>
<td width="60%">
<b>ulDataRedundancyMin</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_DATA_RDNCY_DEF"></a><a id="vds_pool_attrib_data_rdncy_def"></a><dl>
<dt><b>VDS_POOL_ATTRIB_DATA_RDNCY_DEF</b></dt>
<dt>0x80L</dt>
</dl>
</td>
<td width="60%">
<b>ulDataRedundancyDefault</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_PKG_RDNCY_MAX"></a><a id="vds_pool_attrib_pkg_rdncy_max"></a><dl>
<dt><b>VDS_POOL_ATTRIB_PKG_RDNCY_MAX</b></dt>
<dt>0x100L</dt>
</dl>
</td>
<td width="60%">
<b>ulPackageRedundancyDefault</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_PKG_RDNCY_MIN"></a><a id="vds_pool_attrib_pkg_rdncy_min"></a><dl>
<dt><b>VDS_POOL_ATTRIB_PKG_RDNCY_MIN</b></dt>
<dt>0x200L</dt>
</dl>
</td>
<td width="60%">
<b>ulPackageRedundancyMin</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_PKG_RDNCY_DEF"></a><a id="vds_pool_attrib_pkg_rdncy_def"></a><dl>
<dt><b>VDS_POOL_ATTRIB_PKG_RDNCY_DEF</b></dt>
<dt>0x400L</dt>
</dl>
</td>
<td width="60%">
<b>ulPackageRedundancyDefault</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_STRIPE_SIZE"></a><a id="vds_pool_attrib_stripe_size"></a><dl>
<dt><b>VDS_POOL_ATTRIB_STRIPE_SIZE</b></dt>
<dt>0x800L</dt>
</dl>
</td>
<td width="60%">
<b>ulStripeSize</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_STRIPE_SIZE_MAX"></a><a id="vds_pool_attrib_stripe_size_max"></a><dl>
<dt><b>VDS_POOL_ATTRIB_STRIPE_SIZE_MAX</b></dt>
<dt>0x1000L</dt>
</dl>
</td>
<td width="60%">
<b>ulStripeSizeMax</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_STRIPE_SIZE_MIN"></a><a id="vds_pool_attrib_stripe_size_min"></a><dl>
<dt><b>VDS_POOL_ATTRIB_STRIPE_SIZE_MIN</b></dt>
<dt>0x2000L</dt>
</dl>
</td>
<td width="60%">
<b>ulStripeSizeMin</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_STRIPE_SIZE_DEF"></a><a id="vds_pool_attrib_stripe_size_def"></a><dl>
<dt><b>VDS_POOL_ATTRIB_STRIPE_SIZE_DEF</b></dt>
<dt>0x4000L</dt>
</dl>
</td>
<td width="60%">
<b>ulDefaultStripeSize</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_NUM_CLMNS"></a><a id="vds_pool_attrib_num_clmns"></a><dl>
<dt><b>VDS_POOL_ATTRIB_NUM_CLMNS</b></dt>
<dt>0x8000L</dt>
</dl>
</td>
<td width="60%">
<b>ulNumberOfColumns</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_NUM_CLMNS_MAX"></a><a id="vds_pool_attrib_num_clmns_max"></a><dl>
<dt><b>VDS_POOL_ATTRIB_NUM_CLMNS_MAX</b></dt>
<dt>0x10000L</dt>
</dl>
</td>
<td width="60%">
<b>ulNumberOfColumnsMax</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_NUM_CLMNS_MIN"></a><a id="vds_pool_attrib_num_clmns_min"></a><dl>
<dt><b>VDS_POOL_ATTRIB_NUM_CLMNS_MIN</b></dt>
<dt>0x20000L</dt>
</dl>
</td>
<td width="60%">
<b>ulNumberOfColumnsMin</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_NUM_CLMNS_DEF"></a><a id="vds_pool_attrib_num_clmns_def"></a><dl>
<dt><b>VDS_POOL_ATTRIB_NUM_CLMNS_DEF</b></dt>
<dt>0x40000L</dt>
</dl>
</td>
<td width="60%">
<b>ulDefaultNumberofColumns</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_DATA_AVL_HINT"></a><a id="vds_pool_attrib_data_avl_hint"></a><dl>
<dt><b>VDS_POOL_ATTRIB_DATA_AVL_HINT</b></dt>
<dt>0x80000L</dt>
</dl>
</td>
<td width="60%">
<b>ulDataAvailabilityHint</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_ACCS_RNDM_HINT"></a><a id="vds_pool_attrib_accs_rndm_hint"></a><dl>
<dt><b>VDS_POOL_ATTRIB_ACCS_RNDM_HINT</b></dt>
<dt>0x100000L</dt>
</dl>
</td>
<td width="60%">
<b>ulAccessRandomnessHint</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_ACCS_DIR_HINT"></a><a id="vds_pool_attrib_accs_dir_hint"></a><dl>
<dt><b>VDS_POOL_ATTRIB_ACCS_DIR_HINT</b></dt>
<dt>0x200000L</dt>
</dl>
</td>
<td width="60%">
<b>ulAccessDirectionHint</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_ACCS_SIZE_HINT"></a><a id="vds_pool_attrib_accs_size_hint"></a><dl>
<dt><b>VDS_POOL_ATTRIB_ACCS_SIZE_HINT</b></dt>
<dt>0x400000L</dt>
</dl>
</td>
<td width="60%">
<b>ulAccessSizeHint</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_ACCS_LTNCY_HINT"></a><a id="vds_pool_attrib_accs_ltncy_hint"></a><dl>
<dt><b>VDS_POOL_ATTRIB_ACCS_LTNCY_HINT</b></dt>
<dt>0x800000L</dt>
</dl>
</td>
<td width="60%">
<b>ulAccessLatencyHint</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_ACCS_BDW_WT_HINT"></a><a id="vds_pool_attrib_accs_bdw_wt_hint"></a><dl>
<dt><b>VDS_POOL_ATTRIB_ACCS_BDW_WT_HINT</b></dt>
<dt>0x1000000L</dt>
</dl>
</td>
<td width="60%">
<b>ulAccessBandwidthWeightHint</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_STOR_COST_HINT"></a><a id="vds_pool_attrib_stor_cost_hint"></a><dl>
<dt><b>VDS_POOL_ATTRIB_STOR_COST_HINT</b></dt>
<dt>0x2000000L</dt>
</dl>
</td>
<td width="60%">
<b>ulStorageCostHint</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_STOR_EFFCY_HINT"></a><a id="vds_pool_attrib_stor_effcy_hint"></a><dl>
<dt><b>VDS_POOL_ATTRIB_STOR_EFFCY_HINT</b></dt>
<dt>0x4000000L</dt>
</dl>
</td>
<td width="60%">
<b>ulStorageEfficiencyHint</b>

</td>
</tr>
<tr>
<td width="40%"><a id="VDS_POOL_ATTRIB_CUSTOM_ATTRIB"></a><a id="vds_pool_attrib_custom_attrib"></a><dl>
<dt><b>VDS_POOL_ATTRIB_CUSTOM_ATTRIB</b></dt>
<dt>0x8000000L</dt>
</dl>
</td>
<td width="60%">
<b>pPoolCustomAttributes</b>

</td>
</tr>
</table>
 


### -field raidType

A  <a href="https://msdn.microsoft.com/c818d8f4-5ae5-4e40-91b9-a4405524066c">VDS_RAID_TYPE</a> enumeration value that specifies the RAID type of the storage pool. If the storage pool does not have a specific RAID type, set this member to <b>VDS_RT_UNKNOWN</b> and  clear the <b>VDS_POOL_ATTRIB_RAIDTYPE</b> attribute flag in the <b>ullAttributeMask</b> member.


### -field busType

A <a href="https://msdn.microsoft.com/4fa1bd7a-c675-4588-8753-2614be444c9c">VDS_STORAGE_BUS_TYPE</a> enumeration value that specifies the bus type of the drives in the storage pool.


### -field pwszIntendedUsage

A string that specifies the usage of the storage pool. Typically, this may indicate the application that is using the storage pool (for example,  "SQL" or "Exchange") or the business function that is using the storage pool (for example, "Finance" or "Human Resources").


### -field bSpinDown

<b>TRUE</b> if the drives in the storage pool spin down automatically to reduce power usage, or <b>FALSE</b> otherwise.


### -field bIsThinProvisioned

<b>TRUE</b> if the storage pool is thin provisioned, or <b>FALSE</b> otherwise. If the pool is thin provisioned, the number of bytes in the consumed space of the pool could be less than the number of bytes in the provisioned space of the pool. (The number of bytes in the provisioned space is stored in the <b>ullProvisionedSpace</b> member of this structure. The number of bytes in the consumed space is stored in the <b>ullTotalConsumedSpace</b> member of the <a href="https://msdn.microsoft.com/2a82e872-2005-4b05-b67a-161b16c4f3aa">VDS_STORAGE_POOL_PROP</a> structure.) When a hardware provider sets this member to <b>TRUE</b>, it must also set the <b>type</b> member of the <b>VDS_STORAGE_POOL_PROP</b> structure to <b>VDS_SPT_CONCRETE</b>.


### -field ullProvisionedSpace

If the pool is thin provisioned, this member specifies the space, in bytes, that is provisioned for the pool. The value of this member must be greater than or equal to the value of the <b>ullTotalConsumedSpace</b> member of the <a href="https://msdn.microsoft.com/2a82e872-2005-4b05-b67a-161b16c4f3aa">VDS_STORAGE_POOL_PROP</a> structure.


### -field bNoSinglePointOfFailure

<b>TRUE</b> if there is no single point of failure in the pool, or <b>FALSE</b> otherwise.


### -field ulDataRedundancyMax

The maximum number of complete copies of the data that can be maintained in this storage pool.


### -field ulDataRedundancyMin

The minimum number of complete copies of the data that can be maintained in this storage pool.


### -field ulDataRedundancyDefault

The default number of complete copies of the data that are maintained in this storage pool.


### -field ulPackageRedundancyMax

The maximum number of drives that can be used in the storage pool to ensure package redundancy. Package redundancy indicates the number of drives that can fail in the storage pool without resulting in a data loss.


### -field ulPackageRedundancyMin

The minimum number of drives that can be used in the storage pool to ensure package redundancy. Package redundancy indicates the number of drives that can fail in the storage pool without resulting in a data loss.


### -field ulPackageRedundancyDefault

The default number of drives that are used in the storage pool to ensure package redundancy. Package redundancy indicates the number of drives that can fail in the storage pool without resulting in a data loss.


### -field ulStripeSize

The mirror or parity stripe size, in bytes, of the storage pool if the pool is striped (with or without parity).


### -field ulStripeSizeMax

The maximum stripe size, in bytes, that is supported by the storage pool.


### -field ulStripeSizeMin

The minimum stripe size, in bytes, that is supported by the storage pool.


### -field ulDefaultStripeSize

The default stripe size, in bytes, that is supported by the storage pool.


### -field ulNumberOfColumns

The number of columns of the storage pool if the pool is striped (with or without parity).


### -field ulNumberOfColumnsMax

The maximum number of columns supported by the storage pool.


### -field ulNumberOfColumnsMin

The minimum number of columns supported by the storage pool.


### -field ulDefaultNumberofColumns

The default number of columns supported by the storage pool.


### -field ulDataAvailabilityHint

A hint from the client that indicates the importance placed on data availability. Values range from 0 (Not Important) to 10 (Very Important).


### -field ulAccessRandomnessHint

A hint from the client that indicates the randomness of data access. Values range from 0 (Entirely Sequential) to 10 (Entirely Random).


### -field ulAccessDirectionHint

A hint from the client that indicates the direction of data access. Values range from 0 (Entirely Read) to 10 (Entirely Write).


### -field ulAccessSizeHint

A hint from the client that indicates the optimal access size in megabytes.


### -field ulAccessLatencyHint

A hint from the client that indicates the importance of access latency to the client. Values range from 0 (Not Important) to 10 (Very Important).


### -field ulAccessBandwidthWeightHint

A hint from the client that indicates the importance of high bandwidth. Values range from 0 (Not Important) to 10 (Very Important).


### -field ulStorageCostHint

A hint from the client that indicates the importance of storage cost to the client. Values range from 0 (Not Important) to 10 (Very Important). If the storage cost is very important to the client, a value of 10 indicates that the client would prefer to provision the pool using lower cost storage.


### -field ulStorageEfficiencyHint

A hint from the client that indicates the importance of storage efficiency to the client. Values range from 0 (Not Important) to 10 (Very Important).


### -field ulNumOfCustomAttributes

The number of custom attributes defined for the storage pool.


### -field pPoolCustomAttributes

An array of <a href="https://msdn.microsoft.com/beea122a-476c-43e0-bb70-2555d4211bf7">VDS_POOL_CUSTOM_ATTRIBUTES</a> structures. Each structure contains a custom attribute that is defined for the storage pool.


### -field bReserved1

This member is reserved for future use. Do not use.


### -field bReserved2

This member is reserved for future use. Do not use.


### -field ulReserved1

This member is reserved for future use. Do not use.


### -field ulReserved2

This member is reserved for future use. Do not use.


### -field ullReserved1

This member is reserved for future use. Do not use.


### -field ullReserved2

This member is reserved for future use. Do not use.


## -remarks



If an attribute is set for a storage pool, that attribute setting must apply to all drive extents that make up the pool.




## -see-also




<a href="https://msdn.microsoft.com/308c9821-927d-4b90-854d-b050f3730c22">IVdsHwProviderStoragePools::QueryStoragePools</a>



<a href="https://msdn.microsoft.com/44906c1f-ecb2-4701-9392-a9b5924e9d65">IVdsStoragePool::GetAttributes</a>
 

 
