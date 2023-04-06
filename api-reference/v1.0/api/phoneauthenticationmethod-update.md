---
title: "Update phoneAuthenticationMethod"
description: "Update a user's phone number associated with a phoneAuthenticationMethod object."
ms.localizationpriority: medium
author: "mmcla"
ms.prod: "identity-and-sign-in"
doc_type: "apiPageType"
---

# Update phoneAuthenticationMethod

Namespace: microsoft.graph

Update a user's phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md) object.

You can't change a phone's type. To change a phone's type, add a new number of the desired type and then delete the object with the original type.

If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

### Permissions acting on self

|Permission type      | Permissions (from least to most privileged)              |
|:---------------------------------------|:-------------------------|
| Delegated (work or school account)     | UserAuthenticationMethod.ReadWrite |
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | Not supported. |

### Permissions acting on other users

|Permission type      | Permissions (from least to most privileged)              |
|:---------------------------------------|:-------------------------|
| Delegated (work or school account)     | UserAuthenticationMethod.ReadWrite.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | UserAuthenticationMethod.ReadWrite.All |

For delegated scenarios where an admin is acting on another user, the admin needs one of the following [Azure AD roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):
* Global administrator
* Privileged authentication administrator
* Authentication administrator

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/authentication/phoneMethods/{id}
PATCH /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
The value of `id` corresponding to the phoneType to update is one of the following:
+ `b6332ec1-7057-4abe-9331-3d72feddfe41` to update the `alternateMobile` **phoneType**.
+ `e37fc753-ff3b-4958-9484-eaa9425c82bc` to update the `office` **phoneType**.
+ `3179e48a-750b-4051-897c-87b9720928f7` to update the `mobile` **phoneType**.

## Request headers

| Name       | Description|
|:-----------|:-----------|
| Authorization | Bearer {token}. Required. |
| Content-type  | application/json. Required. |

## Request body

In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will be recalculated based on changes to other property values.

| Property     | Type        | Description |
|:-------------|:------------|:------------|
|phoneNumber|String|The phone number to text or call for authentication. Phone numbers use the format `+{country code} {number}x{extension}`, with extension optional. For example, `+1 5555551234` or `+1 5555551234x123` are valid. Numbers are rejected when creating or updating if they do not match the required format.|
|phoneType|string| Possible values are: `mobile`, `alternateMobile`, or `office`.|

## Response

If successful, this method returns a `204 No Content` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.

## Examples

### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-phoneauthenticationmethod-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-phoneauthenticationmethod-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-phoneauthenticationmethod-cli-snippets.md)]
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
  "description": "Update phoneauthenticationmethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
