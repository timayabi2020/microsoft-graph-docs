---
title: "Get domain"
description: "Retrieve the properties and relationships of domain object."
author: "adimitui"
ms.localizationpriority: medium
ms.prod: "directory-management"
doc_type: apiPageType
---

# Get domain

Namespace: microsoft.graph

Retrieve the properties and relationships of domain object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).


|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All  |

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> For {id}, specify the domain with its fully qualified domain name.

## Optional query parameters

This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.

## Request headers

| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer {token}. Required. |
| Content-Type  | application/json |

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.
## Example
##### Request


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["M365x214355.onmicrosoft.com"],
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/M365x214355.onmicrosoft.com
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-domain-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-domain-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-domain-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### Response
Note: The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#domains/$entity",
    "authenticationType": "Managed",
    "availabilityStatus": null,
    "id": "M365x214355.onmicrosoft.com",
    "isAdminManaged": true,
    "isDefault": true,
    "isInitial": true,
    "isRoot": true,
    "isVerified": true,
    "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
    ],
    "passwordValidityPeriodInDays": null,
    "passwordNotificationWindowInDays": null,
    "state": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
