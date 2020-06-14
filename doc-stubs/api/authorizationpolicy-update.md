---
title: "Update authorizationPolicy"
description: "Update the properties of an authorizationPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update authorizationPolicy
Namespace: microsoft.graph

Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /authorizationPolicy
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [authorizationPolicy](../resources/authorizationpolicy.md) object.

The following table shows the properties that are required when you create the [authorizationPolicy](../resources/authorizationpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|blockMsolPowerShell|Boolean|**TODO: Add Description**|
|enabledPreviewFeatures|String collection|**TODO: Add Description**|
|guestUserRoleId|Guid|**TODO: Add Description**|
|permissionGrantPolicyIdsAssignedToDefaultUserRole|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_authorizationpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/authorizationPolicy
Content-Type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.authorizationPolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "blockMsolPowerShell": "Boolean",
  "enabledPreviewFeatures": [
    "String"
  ],
  "guestUserRoleId": "Guid",
  "permissionGrantPolicyIdsAssignedToDefaultUserRole": [
    "String"
  ]
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.authorizationPolicy",
  "id": "5f2d5fd2-5fd2-5f2d-d25f-2d5fd25f2d5f",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "blockMsolPowerShell": "Boolean",
  "enabledPreviewFeatures": [
    "String"
  ],
  "guestUserRoleId": "Guid",
  "permissionGrantPolicyIdsAssignedToDefaultUserRole": [
    "String"
  ]
}
```
