---
title: "Delete personName"
description: "Delete personName object from a user's profile."
ms.localizationpriority: medium
author: "kevinbellinger"
ms.prod: "people"
doc_type: "apiPageType"
---

# Delete personName

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete a [personName](../resources/personname.md) object from a user's [profile](../resources/profile.md).

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | User.ReadWrite, User.ReadWrite.All          |
| Delegated (personal Microsoft account) | User.ReadWrite, User.ReadWrite.All          |
| Application                            | User.ReadWrite.All                          |

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/names/{id}
DELETE /users/{id | userPrincipalName}/profile/names/{id}
```

## Request headers

| Name           |Description                  |
|:---------------|:----------------------------|
| Authorization  | Bearer {token}. Required.   |
| Content-Type   | application/json. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns `204 No Content` response code. It does not return anything in the response body.

## Examples

### Request

The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personname"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/names/{id}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-personname-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/delete-personname-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response


The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


