---
title: "Update directory"
description: "Update the properties of a directory object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update directory
Namespace: microsoft.graph

Update the properties of a directory object.

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
PATCH /roleManagement/directory
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [rbacApplication](../resources/rbacapplication.md) object.

The following table shows the properties that are required when you create the [rbacApplication](../resources/rbacapplication.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response

If successful, this method returns a `200 OK` response code and an updated [rbacApplication](../resources/rbacapplication.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directory"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory
Content-Type: application/json
Content-length: 57

{
  "@odata.type": "#microsoft.graph.rbacApplication"
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
  "@odata.type": "#microsoft.graph.rbacApplication",
  "id": "e08ba21d-a21d-e08b-1da2-8be01da28be0"
}
```
