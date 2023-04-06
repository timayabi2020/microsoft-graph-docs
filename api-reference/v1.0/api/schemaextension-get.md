---
title: "Get schemaExtension"
description: "Get the properties of the specified schemaExtension definition."
ms.localizationpriority: medium
author: "dkershaw10"
ms.prod: "extensions"
doc_type: apiPageType
---

# Get schemaExtension

Namespace: microsoft.graph
Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).


|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | User.Read, Application.Read.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Application.Read.All |

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.

## Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer {token}. Required. |
| Content-Type   | application/json |

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.
## Example
### Request
The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension_extcivhhslh_sbtest1",
  "sampleKeys": ["extcivhhslh_sbtest1"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/schemaExtensions/extcivhhslh_sbtest1
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-schemaextension-extcivhhslh-sbtest1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-schemaextension-extcivhhslh-sbtest1-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-schemaextension-extcivhhslh-sbtest1-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response
The following is an example of the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#schemaExtensions/$entity",
    "id": "extcivhhslh_sbtest1",
    "description": "SbGraph test extensions",
    "targetTypes": [
        "contact",
        "group"
    ],
    "status": "Available",
    "owner": "da033fe6-d48e-435d-8014-e98a4b166900",
    "properties": [
        {
            "name": "customerType",
            "type": "String"
        }
    ]
}
```

## See also

- [Add custom data to resources using extensions](/graph/extensibility-overview)
- [Add custom data to groups using schema extensions](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
