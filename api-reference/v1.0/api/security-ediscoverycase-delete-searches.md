---
title: "Delete ediscoverySearch"
description: "Delete an ediscoverySearch object."
author: "SeunginLyu"
ms.localizationpriority: medium
ms.prod: "ediscovery"
doc_type: "apiPageType"
---

# Delete ediscoverySearch
Namespace: microsoft.graph.security



Delete an [ediscoverySearch](../resources/security-ediscoverysearch.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Not supported.|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}
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
The following is an example of a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_ediscoverysearch"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/58399dff-cebe-478f-b1af-d3227f1fd645/searches/60150269-9758-4439-9bc4-453c864d082f
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-ediscoverysearch-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/delete-ediscoverysearch-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/delete-ediscoverysearch-cli-snippets.md)]
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

