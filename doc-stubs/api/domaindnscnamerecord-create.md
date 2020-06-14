---
title: "Create domainDnsCnameRecord"
description: "Create a new domainDnsCnameRecord object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create domainDnsCnameRecord
Namespace: microsoft.graph

Create a new [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.

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
POST ** Collection URI for microsoft.graph.domainDnsCnameRecord not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.

The following table shows the properties that are required when you create the [domainDnsCnameRecord](../resources/domaindnscnamerecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|recordType|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|supportedService|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|ttl|Int32|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|canonicalName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_domaindnscnamerecord_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.domainDnsCnameRecord not found
Content-Type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.domainDnsCnameRecord",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer",
  "canonicalName": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domaindnscnamerecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.domainDnsCnameRecord",
  "id": "a5a18c37-8c37-a5a1-378c-a1a5378ca1a5",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer",
  "canonicalName": "String"
}
```
