---
title: "Curricula: Pin the unit created"
description: "Pin the created unit for curricula services"
ms.localizationpriority: medium
author: "AsBansal1"
ms.prod: "education"
doc_type: apiPageType
---

# Curricula: Pin and Unpin the unit created

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Pin the unit created for [curricula services](../resources/educationassignment.md). Only teachers can perform this operation.

The teacher determines the unit is to be pinned or unpinned for course outline.

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
POST /education/classes/{id}/units
```
## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |
| Content-Type   | application/json. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [curricula services](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) object in the request body.

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
  "sampleKeys": ["1e40c4aa-98b0-400a-8570-161e8dcfa631", "3258cb60-01dc-439d-9276-4e3b200cdfb9"],
  "name": "curricula_pinunit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/1e40c4aa-98b0-400a-8570-161e8dcfa631/units/3258cb60-01dc-439d-9276-4e3b200cdfb9/pin
Content-type: application/json
```

### Response
The following is an example of the response. 

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationUnit",
    "@odata.type": "#microsoft.graph.educationUnit",
    "displayName": "Conceptual Physics",
    "description": "This chapter will coverconcepts of everyday Physics",
    "resourcesFolderUrl": null,
    "isPinned": true,
    "status": "draft",
    "createdDateTime": "2023-03-15T17:38:45.007054Z",
    "lastModifiedDateTime": "2023-03-15T17:43:08.3512188Z",
    "id": "3258cb60-01dc-439d-9276-4e3b200cdfb9",
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

