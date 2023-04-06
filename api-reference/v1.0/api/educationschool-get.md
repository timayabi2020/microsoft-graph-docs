---
title: "Get educationSchool"
description: "Read the properties and relationships of an educationSchool object."
author: "mlafleur"
ms.localizationpriority: medium
ms.prod: "education"
doc_type: apiPageType
---

# Get educationSchool

Namespace: microsoft.graph

Read the properties and relationships of an [educationSchool](../resources/educationschool.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     | EduRoster.ReadBasic                         |
| Delegated (personal Microsoft account) | Not supported.                              |
| Application                            | EduRoster.Read.All, EduRoster.ReadWrite.All |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}
```

## Optional query parameters

This method supports the same OData query parameters as [Get User](../api/user-get.md#optional-query-parameters). For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.

## Examples

### Request


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/f2598f43-629c-4ea9-9265-97a34839644e
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-educationschool-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-educationschool-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-educationschool-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/schools/$entity",
    "id": "f2598f43-629c-4ea9-9265-97a34839644e",
    "displayName": "Business Training Camp",
    "description": null,
    "principalEmail": "aroebuck@principal.edu",
    "principalName": "Amy Roebuck",
    "externalPrincipalId": "14007",
    "externalId": "10001",
    "externalSource": "sis",
    "externalSourceDetail": "SIS",
    "phone": "555-123-4567",
    "address": {
        "city": "Redmond",
        "countryOrRegion": "US",
        "postalCode": "98052",
        "state": "WA",
        "street": "2 Microsoft Way"
    }
}
```
