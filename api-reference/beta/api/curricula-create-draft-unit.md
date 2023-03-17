---
title: "Curricula: Create draft unit"
description: "Create a new draft unit for the curricula services"
ms.localizationpriority: medium
author: "AsBansal1"
ms.prod: "education"
doc_type: apiPageType
---

# Curricula: Create draft unit

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new draft unit for the [curricula services](../resources/educationassignment.md). Only teachers can perform this operation.

The teacher determines the unit name and description for the class.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) |  EduAssignments.ReadBasic, EduAssignments.Read  |
|Delegated (personal Microsoft account) |  Not supported.  |
|Application | Not supported. | 

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/units//units/{unitId}/resources
```
## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |
| Content-Type   | application/json. Required. |

## Request body
In the request body, supply these values

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|displayName|String| Name of the `unit`.|
|@odata.type|String| The OData entity type in Microsoft Graph that describes the represented object.|
|@odata.id|String| The OData identifier of the object.|

## Response
If successful, this method returns a `201 OK` response code and [curricula services](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) object in the request body.

## Example

### Request
The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["## Example
### Request
The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["1e40c4aa-98b0-400a-8570-161e8dcfa631"],
  "name": "curricula_creatdraftunit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/1e40c4aa-98b0-400a-8570-161e8dcfa631/units
Content-type: application/json

{
    "displayName": "Conceptual Physics",
    "description": "This chapter will cover concepts of everyday Physics"
}
```

### Response
The following is an example of the response. 

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('1e40c4aa-98b0-400a-8570-161e8dcfa631')/units/$entity",
    "displayName": "Conceptual Physics",
    "description": "This chapter will cover concepts of everyday Physics",
    "resourcesFolderUrl": null,
    "isPinned": false,
    "status": "draft",
    "createdDateTime": "2023-03-15T15:37:43.6091261Z",
    "lastModifiedDateTime": "2023-03-15T15:37:43.6248439Z",
    "id": "8be88b49-7857-4d26-bc13-c31f083bef80",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
            "displayName": null
        }
    }
}
```
