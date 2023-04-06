---
title: "Get appConsentRequest"
description: "Read the properties and relationships of an appConsentRequest object."
author: "psignoret"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---

# Get appConsentRequest

Namespace: microsoft.graph

Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|ConsentRequest.Read.All, ConsentRequest.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|ConsentRequest.Read.All, ConsentRequest.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}
```

## Optional query parameters

This method supports the `$select` OData query parameter to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [appConsentRequest](../resources/appconsentrequest.md) object in the response body.

## Examples

### Request


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests/7322e5f3-0f15-4eb8-9e82-2029e8622f5d
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-appconsentrequest-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-appconsentrequest-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-appconsentrequest-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appConsentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests/$entity",
    "id": "7322e5f3-0f15-4eb8-9e82-2029e8622f5d",
    "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
    "appDisplayName": "Graph Explorer",
    "consentType": "Dynamic",
    "pendingScopes": [],
    "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('7322e5f3-0f15-4eb8-9e82-2029e8622f5d')/userConsentRequests",
    "userConsentRequests": []
}
```
