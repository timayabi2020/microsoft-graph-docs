---
title: "Close Session"
description: "Use this API to close an existing workbook session. "
author: "lumine2008"
ms.localizationpriority: medium
ms.prod: "excel"
doc_type: apiPageType
---

# Close Session

Namespace: microsoft.graph

Use this API to close an existing workbook session.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Files.ReadWrite    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Not supported. |

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/closeSession
POST /me/drive/root:/{item-path}:/workbook/closeSession
workbook-session-id: {session-id}
```
## Request headers
| Name                | Description                      |
|:--------------------|:---------------------------------|
| Authorization       | Bearer {token}. Required.        |
| workbook-session-id | Workbook session Id to be closed |

## Request body
This API does not require any request body.

## Response

If successful, this method returns `204 No Content` response code.

## Example
##### Request
Here is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}

{

}
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/close-excel-session-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/close-excel-session-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Note that workbook-session-id header is required.


##### Response
Here is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
  ]
}-->

