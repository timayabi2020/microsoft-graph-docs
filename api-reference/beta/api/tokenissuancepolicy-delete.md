---
title: "Delete tokenIssuancePolicy"
description: "Delete tokenIssuancePolicy."
ms.localizationpriority: medium
author: "luleonpla"
ms.prod: "identity-and-sign-in"
doc_type: "apiPageType"
---

# Delete tokenIssuancePolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | Policy.ReadWrite.ApplicationConfiguration |
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | Policy.ReadWrite.ApplicationConfiguration |

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenIssuancePolicies/{id}
```

## Request headers

| Name          | Description   |
|:--------------|:--------------|
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-tokenissuancepolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/delete-tokenissuancepolicy-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


