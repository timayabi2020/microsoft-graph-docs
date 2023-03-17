---
title: "Curricula: Add unit resource"
description: "Use curricula services to add any resource type (word, excel, file, link, powerpoint or assignment resource) to a unit"
ms.localizationpriority: medium
author: "AsBansal1"
ms.prod: "education"
doc_type: apiPageType
---

# Curricula: Get pinned units

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use [curricula services](../resources/educationassignment.md) to add any resource type (word, excel, file, link, powerpoint or assignment resource) to a unit.

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
POST /education/classes/{id}/units/{{unitId}}/resources
```
## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |
| Content-Type   | application/json. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code.

## Examples

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
  "name": "curricula_setupresourcesfolder"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/1e40c4aa-98b0-400a-8570-161e8dcfa631/units/b9f96874-8b86-4b5f-9885-63590a8f60e8/setUpResourcesFolder
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationUnit",
    "@odata.type": "#microsoft.graph.educationUnit",
    "displayName": "Conceptual Physics",
    "description": "This chapter will coverconcepts of everyday Physics",
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!UmWjcTCfj0iEQfUkbqAaIUQ4l046NrNIq092DJz8KtOU7DSL1lweS7rmmZDVXd8W/items/01OMTFXGZDSF6JTYDVF5FLOGSQKHVASTM2",
    "isPinned": false,
    "status": "draft",
    "createdDateTime": "2023-03-15T22:16:29.8844326Z",
    "lastModifiedDateTime": "2023-03-15T22:49:47.2636145Z",
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