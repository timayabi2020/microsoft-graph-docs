---
title: "List memberOf"
description: "List the groups that this organizaitonal contact is a member of."
ms.localizationpriority: medium
author: "dkershaw10"
ms.prod: "directory-management"
doc_type: apiPageType
---

# List memberOf

Namespace: microsoft.graph

List the groups that this [organizational contact](../resources/orgcontact.md) is a member of.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | OrgContact.Read.All and Group.Read.All, Directory.Read.All  |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | OrgContact.Read.All and Group.Read.All, Directory.Read.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) `$select` to help customize the response.

## Request headers
| Header       | Value |
|:-----------|:----------|
| Authorization  | Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.
## Example
##### Request
The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/e63333f5-3d11-4026-8fe3-c0f7b044dd3a/memberOf
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/contact-get-memberof-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/contact-get-memberof-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/contact-get-memberof-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### Response
The following is an example of the response.
>**Note**: The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "024bbfa0-fe5a-4fce-9227-bd6ccf1324bb",
      "createdDateTime": "2018-01-18T18:54:43Z",
      "description": "Best group ever created",
      "displayName": "Best Group",
      "groupTypes": [],
      "isAssignableToRole": null,
      "onPremisesProvisioningErrors": []
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
