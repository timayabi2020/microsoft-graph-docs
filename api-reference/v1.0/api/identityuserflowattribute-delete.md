---
title: "Delete identityUserFlowAttribute"
description: "Delete an identityUserFlowAttribute."
ms.localizationpriority: medium
doc_type: apiPageType
author: "jkdouglas"
ms.prod: "identity-and-sign-in"
---

# Delete identityUserFlowAttribute

Namespace: microsoft.graph

Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md). Only custom user flow attributes can be deleted.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account)|IdentityUserFlow.ReadWrite.All|
|Delegated (personal Microsoft account)| Not supported.|
|Application|IdentityUserFlow.ReadWrite.All|

The work or school account needs to belong to one of the following roles:

* Global administrator
* External Identity User Flow Attribute administrator

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## Request headers

|Name|Description|
|:---------------|:----------|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns `204 No Content` response code.

## Example

### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes",
  "sampleKeys": ["extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby"]
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-userflowattributes-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/delete-userflowattributes-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/delete-userflowattributes-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
