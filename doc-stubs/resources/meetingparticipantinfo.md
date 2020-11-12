---
title: "meetingParticipantInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# meetingParticipantInfo resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|identity|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|role|onlineMeetingRole|**TODO: Add Description**. Possible values are: `attendee`, `presenter`, `unknownFutureValue`.|
|upn|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingParticipantInfo",
  "identity": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "upn": "String",
  "role": "String"
}
```
