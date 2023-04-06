---
title: 'Get applicationTemplate'
description: 'Retrieve the properties and relationships of applicationtemplate object.'
ms.localizationpriority: medium
author: 'luleonpla'
ms.prod: 'applications'
doc_type: apiPageType
---

# Get applicationTemplate

Namespace: microsoft.graph

Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     | None.                                       |
| Delegated (personal Microsoft account) | Not supported.                              |
| Application                            | None.                                       |

Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## Optional query parameters

You can use a `$select` query parameter to specify only the properties you need for best performance. The **id** property is always returned.

For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description   |
| :------------ | :------------ |
| Authorization | Bearer {code} |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.

## Examples

### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applicationTemplates/4f2fc37d-967b-4929-9959-fbe9c9dbccca
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-applicationtemplate-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-applicationtemplate-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-applicationtemplate-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

The following is an example of the response.

> **Note:** The response object shown here might be shortened for readability. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
	"id" : "id-value",
	"displayName" : "displayName-value",
	"homePageUrl" : "homePageUrl-value",
	"supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
	"logoUrl" : "logoUrl-value",
	"categories" : ["categories-value"],
	"publisher" : "publisher-value",
	"description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
