---
title: "Delete organizationalBranding"
description: "Deletes an organizationalBranding object."
author: "AlexanderMars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Delete organizationalBranding
Namespace: microsoft.graph

Delete the default organizational branding object. To delete the [organizationalBranding](../resources/organizationalbranding.md) object, all images (Stream types) must first be removed from the object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|Organization.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Not supported.|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /organization/{organizationId}/branding
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

In the request body, supply a JSON representation of the default [organizationalBranding](../resources/organizationalbranding.md) object. only the **id** property is required.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbranding"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding

{
    "id": "0"
}
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/delete-organizationalbranding-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/delete-organizationalbranding-cli-snippets.md)]
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

