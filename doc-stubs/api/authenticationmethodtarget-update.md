---
title: "Update authenticationMethodTarget"
description: "Update the properties of an authenticationMethodTarget object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update authenticationMethodTarget
Namespace: microsoft.graph

Update the properties of an [authenticationMethodTarget](../resources/authenticationmethodtarget.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

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
PATCH /authenticationMethodTarget
PATCH /qrAuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
PATCH /fido2AuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
PATCH /emailAuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
PATCH /voiceAuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
PATCH /passwordAuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
PATCH /hardwareOathAuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
PATCH /softwareOathAuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
PATCH /temporaryAccessPassAuthenticationMethodConfiguration/includeTargets/{authenticationMethodTargetId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [authenticationMethodTarget](../resources/authenticationmethodtarget.md) object.

The following table shows the properties that are required when you update the [authenticationMethodTarget](../resources/authenticationmethodtarget.md).

|Property|Type|Description|
|:---|:---|:---|
|targetType|authenticationMethodTargetType|**TODO: Add Description**. Possible values are: `user`, `group`, `unknownFutureValue`.|
|id|String|**TODO: Add Description**|
|isRegistrationRequired|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [authenticationMethodTarget](../resources/authenticationmethodtarget.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_authenticationmethodtarget"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/authenticationMethodTarget
Content-Type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "targetType": "String",
  "isRegistrationRequired": "Boolean"
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
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "targetType": "String",
  "id": "f9832d07-2d07-f983-072d-83f9072d83f9",
  "isRegistrationRequired": "Boolean"
}
```
