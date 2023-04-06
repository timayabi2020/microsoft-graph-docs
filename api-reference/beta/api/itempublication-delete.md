---
title: "Delete itemPublication"
description: "Deletes an itemPublication object."
ms.localizationpriority: medium
author: "kevinbellinger"
ms.prod: "people"
doc_type: apiPageType
---

# Delete itemPublication

Namespace: microsoft.graph

Deletes an [itemPublication](../resources/itempublication.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Delegated (work or school account)     | User.ReadWrite, User.ReadWrite.All |
| Delegated (personal Microsoft account) | User.ReadWrite, User.ReadWrite.All |
| Application                            | User.ReadWrite.All                            |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/publications/{id}
DELETE /users/{id | userPrincipalName}/profile/publications/{id}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request
# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemPublication"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/publications/{id}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-itempublication-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/delete-itempublication-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


