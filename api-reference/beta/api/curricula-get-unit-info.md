---
title: "Curricula: Get unit information"
description: "Get an information on the current unit"
ms.localizationpriority: medium
author: "AshwaniBansal1"
ms.prod: "education"
doc_type: apiPageType
---

# Curricula: Create draft unit

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get an information on the current unit being used in the class for [curricula services](../resources/educationassignment.md). 

This operation can be performed by the teachers and students.

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
  "sampleKeys": ["1e40c4aa-98b0-400a-8570-161e8dcfa631", "b9f96874-8b86-4b5f-9885-63590a8f60e8"],
  "name": "curricula_getunitinfo"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/1e40c4aa-98b0-400a-8570-161e8dcfa631/units/b9f96874-8b86-4b5f-9885-63590a8f60e8
Content-type: application/json

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('1e40c4aa-98b0-400a-8570-161e8dcfa631')/units/$entity",
    "displayName": "Conceptual Physics",
    "description": "This chapter will coverconcepts of everyday Physics",
    "resourcesFolderUrl": null,
    "isPinned": false,
    "status": "draft",
    "createdDateTime": "2023-03-15T22:16:29.8844326Z",
    "lastModifiedDateTime": "2023-03-15T22:16:29.9000487Z",
    "id": "b9f96874-8b86-4b5f-9885-63590a8f60e8",
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
