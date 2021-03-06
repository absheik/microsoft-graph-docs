---
title: "List comanagementEligibleDeviceEntity"
description: "List properties and relationships of the comanagementEligibleDeviceEntity objects."
author: "rolyon"
localization_priority: Normal
ms.prod: "Intune"
doc_type: apiPageType
---

# List comanagementEligibleDeviceEntity

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

List properties and relationships of the comanagementEligibleDeviceEntity objects.

## Prerequisites
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleReports
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of comanagementEligibleDeviceEntity objects in the response body.

## Example

### Request
Here is an example of the request.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleReports
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
	  "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
	  "id": "659554f2-54f2-6595-f254-9565f2549565",
	  "deviceId": "Device Id value",
	  "deviceName": "Device Name value",
	  "deviceType": "Device Type value",
	  "clientRegistrationStatus": "Client Registration Status value",
	  "ownerType": "Owner Type value",
	  "managementAgents": "Management Agent value",
	  "managementState": "Management State value",
	  "referenceId": "Reference Id value",
	  "mdmStatus": "MDM Status value",
	  "osVersion": "OS Version value",
	  "serialNumber": "Serial Number value",
	  "manufacturer": "Manufacture value",
	  "model": "Model value",
	  "osDescription": "OS Description value",
	  "entitySource": 1024,
	  "userId": "User Id value",
	  "upn": "UPN value",
	  "userEmail": "User Email value",
	  "userName": "User name value",
	  "coManageEligibleStatus": "CO Manage Eligible Status value"
    }
  ]
}
```



