---
title: "Update endpoints"
description: "Update the properties of an endpoints object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update endpoints
Namespace: microsoft.graph

Update the properties of an endpoints object.

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
PATCH /groups/{groupsId}/endpoints
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [endpoint](../resources/endpoint.md) object.

The following table shows the properties that are required when you create the [endpoint](../resources/endpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|capability|String|**TODO: Add Description**|
|providerId|String|**TODO: Add Description**|
|providerName|String|**TODO: Add Description**|
|uri|String|**TODO: Add Description**|
|providerResourceId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [endpoint](../resources/endpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_endpoints"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/endpoints
Content-Type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.endpoint",
  "deletedDateTime": "String (timestamp)",
  "capability": "String",
  "providerId": "String",
  "providerName": "String",
  "uri": "String",
  "providerResourceId": "String"
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
  "@odata.type": "#microsoft.graph.endpoint",
  "id": "936d5d6b-5d6b-936d-6b5d-6d936b5d6d93",
  "deletedDateTime": "String (timestamp)",
  "capability": "String",
  "providerId": "String",
  "providerName": "String",
  "uri": "String",
  "providerResourceId": "String"
}
```
