---
title: "Create documentSetVersion"
description: "Create a new version of a document set item in a list."
author: "swapnil1993"
ms.localizationpriority: medium
ms.prod: "sites-and-lists"
doc_type: apiPageType
---

# Create documentSetVersion
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [version of a document set](../resources/documentsetversion.md) item in a [list](../resources/list.md).

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All, Sites.Selected|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/documentSetVersions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [documentSetVersion](../resources/documentsetversion.md) object.

You can specify the following properties when you create a **documentSetVersion**.

|Property|Type|Description|
|:---|:---|:---|
|comment|String|Comment about the captured version. Optional.|
|shouldCaptureMinorVersion|Boolean|If `true`, minor versions of items are also captured; otherwise, only major versions will be captured. Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [documentSetVersion](../resources/documentsetversion.md) object in the response body.

## Examples

### Request

The following is an example of a request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_documentsetversion",
  "sampleKeys": ["2", "root", "Documents"]
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/root/lists/Documents/items/2/documentSetVersions
Content-Type: application/json
Content-length: 70

{
  "comment": "v1",
  "shouldCaptureMinorVersion": false
}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-documentsetversion-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/create-documentsetversion-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### Response

The following is an example of the response.

>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "name": "create_documentsetversion",
  "truncated": true,
  "@odata.type": "microsoft.graph.documentSetVersion"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "1",
    "lastModifiedDateTime": "2022-04-05T04:53:42Z",
    "comment": "v1",
    "createdDateTime": "2022-04-05T04:53:42Z",
    "shouldCaptureMinorVersion": false,
    "lastModifiedBy": {
        "user": {
            "displayName": "Tenant Admin User",
            "email": "admin@contoso.sharepoint.com"
        }
    },
    "items": [
        {
            "itemId": "a5d83ae7-8c3e-4a2c-bc3e-8f276db857bf",
            "versionId": "1.0"
        }
    ],
    "createdBy": {
        "user": {
            "displayName": "Tenant Admin User",
            "email": "admin@contoso.sharepoint.com"
        }
    }
}
```

