---
UID: NS:winsvc._SERVICE_TRIGGER
title: SERVICE_TRIGGER
author: windows-sdk-content
description: Represents a service trigger event. This structure is used by the SERVICE_TRIGGER_INFO structure.
old-location: base\service_trigger.htm
tech.root: services
ms.assetid: a57aa702-40a2-4880-80db-6c4f43c3e7ea
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: "*PSERVICE_TRIGGER, DOMAIN_JOIN_GUID, DOMAIN_LEAVE_GUID, FIREWALL_PORT_CLOSE_GUID, FIREWALL_PORT_OPEN_GUID, MACHINE_POLICY_PRESENT_GUID, NAMED_PIPE_EVENT_GUID, NETWORK_MANAGER_FIRST_IP_ADDRESS_ARRIVAL_GUID, NETWORK_MANAGER_LAST_IP_ADDRESS_REMOVAL_GUID, PSERVICE_TRIGGER, PSERVICE_TRIGGER structure pointer, RPC_INTERFACE_EVENT_GUID, SERVICE_TRIGGER, SERVICE_TRIGGER structure, SERVICE_TRIGGER_ACTION_SERVICE_START, SERVICE_TRIGGER_ACTION_SERVICE_STOP, SERVICE_TRIGGER_TYPE_CUSTOM, SERVICE_TRIGGER_TYPE_DEVICE_INTERFACE_ARRIVAL, SERVICE_TRIGGER_TYPE_DOMAIN_JOIN, SERVICE_TRIGGER_TYPE_FIREWALL_PORT_EVENT, SERVICE_TRIGGER_TYPE_GROUP_POLICY, SERVICE_TRIGGER_TYPE_IP_ADDRESS_AVAILABILITY, SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT, USER_POLICY_PRESENT_GUID, base.service_trigger, winsvc/PSERVICE_TRIGGER, winsvc/SERVICE_TRIGGER"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: winsvc.h
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
 - winsvc.h
api_name:
 - SERVICE_TRIGGER
product: Windows
targetos: Windows
req.typenames: SERVICE_TRIGGER, *PSERVICE_TRIGGER
req.redist: 
---

# SERVICE_TRIGGER structure


## -description


Represents a service trigger event. This structure is used by the <a href="https://msdn.microsoft.com/8de46056-1ea5-46f2-a260-ad140fd77bc1">SERVICE_TRIGGER_INFO</a> structure. 


## -struct-fields




### -field dwTriggerType

The trigger event type. This member can be one of the following values. 

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_TYPE_CUSTOM"></a><a id="service_trigger_type_custom"></a><dl>
<dt><b>SERVICE_TRIGGER_TYPE_CUSTOM</b></dt>
<dt>20</dt>
</dl>
</td>
<td width="60%">
The event is a custom event generated by an <a href="http://go.microsoft.com/fwlink/p/?linkid=133390">Event Tracing for Windows</a> (ETW) provider.  This trigger event can be used to start or stop a service.

The <b>pTriggerSubtype</b> member specifies the event provider's GUID.

The <b>pDataItems</b> member specifies trigger-specific data defined by the provider.

</td>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_TYPE_DEVICE_INTERFACE_ARRIVAL"></a><a id="service_trigger_type_device_interface_arrival"></a><dl>
<dt><b>SERVICE_TRIGGER_TYPE_DEVICE_INTERFACE_ARRIVAL</b></dt>
<dt>1</dt>
</dl>
</td>
<td width="60%">
The event is triggered when a device of the specified device interface class arrives or is present when the system starts.  This trigger event is  commonly used to start a service. 

The <b>pTriggerSubtype</b> member specifies the device interface class GUID. These GUIDs are defined in device-specific header files provided with the <a href="http://go.microsoft.com/fwlink/p/?linkid=133480">Windows Driver Kit</a> (WDK). 

The <b>pDataItems</b> member specifies one or more hardware ID and compatible ID strings for the device interface class.  Strings must be Unicode. If more than one string is specified, the event is triggered if any one of the strings match. For example,  the Wpdbusenum service is started when a device  of device interface class  GUID_DEVINTERFACE_DISK {53f56307-b6bf-11d0-94f2-00a0c91efb8b} and a hardware ID string of <code>"USBSTOR\GenDisk"</code> arrives.

</td>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_TYPE_DOMAIN_JOIN"></a><a id="service_trigger_type_domain_join"></a><dl>
<dt><b>SERVICE_TRIGGER_TYPE_DOMAIN_JOIN</b></dt>
<dt>3</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the computer joins or leaves   a domain. This trigger event can be used to start or stop a service.

The <b>pTriggerSubtype</b> member specifies DOMAIN_JOIN_GUID or DOMAIN_LEAVE_GUID. 

The <b>pDataItems</b> member is not used. 

</td>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_TYPE_FIREWALL_PORT_EVENT"></a><a id="service_trigger_type_firewall_port_event"></a><dl>
<dt><b>SERVICE_TRIGGER_TYPE_FIREWALL_PORT_EVENT</b></dt>
<dt>4</dt>
</dl>
</td>
<td width="60%">
The event is triggered when a firewall port is opened or approximately 60 seconds after the firewall port is closed. This trigger event can be used to start or stop a service.

The <b>pTriggerSubtype</b> member specifies FIREWALL_PORT_OPEN_GUID or FIREWALL_PORT_CLOSE_GUID. 

The <b>pDataItems</b> member specifies the port, the protocol, and optionally the executable path and user information (SID string or name) of the service listening on the event. The "RPC" token can be used in place of the port to specify any listening socket used by RPC. The "system" token can be used in place of the executable path to specify ports created by and listened on by the Windows kernel.

The event is triggered only if all strings match. For example, if MyService hosted inside MyServiceProcess.exe is to be trigger-started when port UDP 5001 opens, the trigger-specific data would be the Unicode representation of <code>"5001\0UDP\0%programfiles%\MyApplication\MyServiceProcess.exe\0MyService\0\0"</code>.

<div class="alert"><b>Note</b>  Before this event can be registered,  the Base Filtering Engine (BFE) service and all services that depend on it must be stopped. After the event is registered, the BFE service and services that depend on it can be restarted. For more information, see Remarks.</div>
<div> </div>
</td>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_TYPE_GROUP_POLICY"></a><a id="service_trigger_type_group_policy"></a><dl>
<dt><b>SERVICE_TRIGGER_TYPE_GROUP_POLICY</b></dt>
<dt>5</dt>
</dl>
</td>
<td width="60%">
The event is triggered when a machine policy or user policy change occurs. This trigger event is  commonly used to start a service.

The <b>pTriggerSubtype</b> member specifies MACHINE_POLICY_PRESENT_GUID or USER_POLICY_PRESENT_GUID. 

The <b>pDataItems</b> member is not used. 

</td>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_TYPE_IP_ADDRESS_AVAILABILITY"></a><a id="service_trigger_type_ip_address_availability"></a><dl>
<dt><b>SERVICE_TRIGGER_TYPE_IP_ADDRESS_AVAILABILITY</b></dt>
<dt>2</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the first IP address on the TCP/IP networking stack becomes available or the last IP address on the stack becomes unavailable. This trigger event can be used to start or stop a service.

The <b>pTriggerSubtype</b> member specifies NETWORK_MANAGER_FIRST_IP_ADDRESS_ARRIVAL_GUID or NETWORK_MANAGER_LAST_IP_ADDRESS_REMOVAL_GUID. 

The <b>pDataItems</b> member is not used. 

</td>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT"></a><a id="service_trigger_type_network_endpoint"></a><dl>
<dt><b>SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT</b></dt>
<dt>6</dt>
</dl>
</td>
<td width="60%">
The event is triggered when a packet or request arrives on a particular network protocol. This request is commonly used to start a service that has stopped itself after an idle time-out when there is no work to do.

<b>Windows 7 and Windows Server 2008 R2:  </b>This trigger type is not supported until Windows 8 and Windows Server 2012.

The <b>pTriggerSubtype</b> member specifies one of the following values: RPC_INTERFACE_EVENT_GUID or NAMED_PIPE_EVENT_GUID.

The <b>pDataItems</b> member specifies an endpoint or interface GUID. The string must be Unicode. The event triggers if the string is an exact match.

The <b>dwAction</b> member must be SERVICE_TRIGGER_ACTION_SERVICE_START.

</td>
</tr>
</table>
 


### -field dwAction

The action to take when the specified trigger event occurs. This member can be one of the following values. 

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_ACTION_SERVICE_START"></a><a id="service_trigger_action_service_start"></a><dl>
<dt><b>SERVICE_TRIGGER_ACTION_SERVICE_START</b></dt>
<dt>1</dt>
</dl>
</td>
<td width="60%">
Start the service when the specified trigger event occurs.

</td>
</tr>
<tr>
<td width="40%"><a id="SERVICE_TRIGGER_ACTION_SERVICE_STOP"></a><a id="service_trigger_action_service_stop"></a><dl>
<dt><b>SERVICE_TRIGGER_ACTION_SERVICE_STOP</b></dt>
<dt>2</dt>
</dl>
</td>
<td width="60%">
Stop the service when the specified trigger event occurs.

</td>
</tr>
</table>
 


### -field pTriggerSubtype

Points to a GUID that identifies the trigger event subtype. The value of this member depends on the value of the <b>dwTriggerType</b> member. 

If <b>dwTriggerType</b> is SERVICE_TRIGGER_TYPE_CUSTOM, <b>pTriggerSubtype</b> is the GUID that identifies the custom event provider. 

If <b>dwTriggerType</b> is SERVICE_TRIGGER_TYPE_DEVICE_INTERFACE_ARRIVAL, <b>pTriggerSubtype</b> is the GUID that identifies the device interface class.

If <b>dwTriggerType</b> is SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT, <b>pTriggerSubtype</b> is one of the following values. 



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="NAMED_PIPE_EVENT_GUID"></a><a id="named_pipe_event_guid"></a><dl>
<dt><b>NAMED_PIPE_EVENT_GUID</b></dt>
<dt>1F81D131-3FAC-4537-9E0C-7E7B0C2F4B55</dt>
</dl>
</td>
<td width="60%">
The event is triggered when a request is made to open the named pipe specified by <b>pDataItems</b>.  The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT.  The <b>dwAction</b> member must be SERVICE_TRIGGER_ACTION_SERVICE_START.

</td>
</tr>
<tr>
<td width="40%"><a id="RPC_INTERFACE_EVENT_GUID"></a><a id="rpc_interface_event_guid"></a><dl>
<dt><b>RPC_INTERFACE_EVENT_GUID</b></dt>
<dt>BC90D167-9470-4139-A9BA-BE0BBBF5B74D</dt>
</dl>
</td>
<td width="60%">
The event is triggered when an endpoint resolution request arrives for the RPC interface GUID specified by <b>pDataItems</b>.  The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT.  The <b>dwAction</b> member must be SERVICE_TRIGGER_ACTION_SERVICE_START.

</td>
</tr>
</table>
 

For other trigger event types, <b>pTriggerSubType</b> can be one of the following values. 

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="DOMAIN_JOIN_GUID"></a><a id="domain_join_guid"></a><dl>
<dt><b>DOMAIN_JOIN_GUID</b></dt>
<dt>1ce20aba-9851-4421-9430-1ddeb766e809</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the computer joins a domain. The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_DOMAIN_JOIN.

</td>
</tr>
<tr>
<td width="40%"><a id="DOMAIN_LEAVE_GUID"></a><a id="domain_leave_guid"></a><dl>
<dt><b>DOMAIN_LEAVE_GUID</b></dt>
<dt>ddaf516e-58c2-4866-9574-c3b615d42ea1</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the computer leaves a domain. The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_DOMAIN_JOIN.

</td>
</tr>
<tr>
<td width="40%"><a id="FIREWALL_PORT_OPEN_GUID"></a><a id="firewall_port_open_guid"></a><dl>
<dt><b>FIREWALL_PORT_OPEN_GUID</b></dt>
<dt>b7569e07-8421-4ee0-ad10-86915afdad09</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the specified firewall port is opened. The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_FIREWALL_PORT_EVENT.

</td>
</tr>
<tr>
<td width="40%"><a id="FIREWALL_PORT_CLOSE_GUID"></a><a id="firewall_port_close_guid"></a><dl>
<dt><b>FIREWALL_PORT_CLOSE_GUID</b></dt>
<dt>a144ed38-8e12-4de4-9d96-e64740b1a524</dt>
</dl>
</td>
<td width="60%">
The event is triggered approximately 60 seconds after the specified firewall port is closed. The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_FIREWALL_PORT_EVENT.

</td>
</tr>
<tr>
<td width="40%"><a id="MACHINE_POLICY_PRESENT_GUID"></a><a id="machine_policy_present_guid"></a><dl>
<dt><b>MACHINE_POLICY_PRESENT_GUID</b></dt>
<dt>659FCAE6-5BDB-4DA9-B1FF-CA2A178D46E0</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the machine policy has changed. The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_GROUP_POLICY.

</td>
</tr>
<tr>
<td width="40%"><a id="NETWORK_MANAGER_FIRST_IP_ADDRESS_ARRIVAL_GUID"></a><a id="network_manager_first_ip_address_arrival_guid"></a><dl>
<dt><b>NETWORK_MANAGER_FIRST_IP_ADDRESS_ARRIVAL_GUID</b></dt>
<dt>4f27f2de-14e2-430b-a549-7cd48cbc8245</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the first IP address on the TCP/IP networking stack becomes available. The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_IP_ADDRESS_AVAILABILITY.

</td>
</tr>
<tr>
<td width="40%"><a id="NETWORK_MANAGER_LAST_IP_ADDRESS_REMOVAL_GUID"></a><a id="network_manager_last_ip_address_removal_guid"></a><dl>
<dt><b>NETWORK_MANAGER_LAST_IP_ADDRESS_REMOVAL_GUID</b></dt>
<dt>cc4ba62a-162e-4648-847a-b6bdf993e335</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the last IP address on the TCP/IP networking stack becomes unavailable. The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_IP_ADDRESS_AVAILABILITY.

</td>
</tr>
<tr>
<td width="40%"><a id="USER_POLICY_PRESENT_GUID"></a><a id="user_policy_present_guid"></a><dl>
<dt><b>USER_POLICY_PRESENT_GUID</b></dt>
<dt>54FB46C8-F089-464C-B1FD-59D1B62C3B50</dt>
</dl>
</td>
<td width="60%">
The event is triggered when the user policy has changed. The <b>dwTriggerType</b> member must be SERVICE_TRIGGER_TYPE_GROUP_POLICY.

</td>
</tr>
</table>
 


### -field cDataItems

The number of <a href="https://msdn.microsoft.com/670e6c49-bbc0-4af6-9e47-6c89801ebb45">SERVICE_TRIGGER_SPECIFIC_DATA_ITEM</a> structures in the array pointed to by <i>pDataItems</i>. 

This member is valid only if the <b>dwDataType</b> member is SERVICE_TRIGGER_TYPE_CUSTOM, SERVICE_TRIGGER_TYPE_DEVICE_ARRIVAL, SERVICE_TRIGGER_TYPE_FIREWALL_PORT_EVENT, or SERVICE_TRIGGER_TYPE_NETWORK_ENDPOINT.


### -field cDataItems.range

 


### -field cDataItems.range.0

 


### -field cDataItems.range.64

 


### -field pDataItems

A pointer to an array of <a href="https://msdn.microsoft.com/670e6c49-bbc0-4af6-9e47-6c89801ebb45">SERVICE_TRIGGER_SPECIFIC_DATA_ITEM</a> structures that contain trigger-specific data. 


### -field pDataItems.size_is

 


### -field pDataItems.size_is.cDataItems

 




## -remarks



On a system that is joined to a domain, security policy settings may prevent the BFE service and its dependent services from being stopped or cause them to restart automatically. In this case, it is necessary to disable the services and then re-enable them after the event is registered. To do this programmatically, store each service's original start type, change the service start type to SERVICE_DISABLED, register the event, and then restore the service's original start type. For information about changing a service's start type, see <a href="https://msdn.microsoft.com/add8a99b-aced-4341-9790-86efac76df6b">ChangeServiceConfig</a>. 

To disable the services using the SC command-line tool, use the  command <b>sc config bfe start= disabled</b>  to disable the BFE service and its dependent services, then use the command <b>net stop bfe /Y</b>  to stop them.  To re-enable the services, use the command <b>sc config bfe start= auto</b>. For more information about the SC command-line tool, see <a href="https://msdn.microsoft.com/7c3e5c39-ec0f-4174-9ecf-239927de3d39">Controlling a Service Using SC</a>.

If it is not possible to disable the services, it may be necessary to restart the system after installing the service that is registering the event. In this case, do not disable the BFE service and its dependent services before restarting the system, because the system may not work correctly if these services remain disabled. 




## -see-also




<a href="https://msdn.microsoft.com/6e5b79ed-52e1-460e-b076-01afbd08775c">ChangeServiceConfig2</a>



<a href="https://msdn.microsoft.com/cb090e59-aeff-4420-bb7c-912a4911006f">QueryServiceConfig2</a>



<a href="https://msdn.microsoft.com/8de46056-1ea5-46f2-a260-ad140fd77bc1">SERVICE_TRIGGER_INFO</a>



<a href="https://msdn.microsoft.com/670e6c49-bbc0-4af6-9e47-6c89801ebb45">SERVICE_TRIGGER_SPECIFIC_DATA_ITEM</a>



<a href="https://msdn.microsoft.com/ca02a3ae-b16a-4427-b6db-b935c9cf23b3">Service Trigger Events</a>
 

 
