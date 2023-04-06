---
title: "Update identityProvider"
description: "Update properties of an identityProvider."
ms.localizationpriority: medium
doc_type: apiPageType
author: "namkedia"
ms.prod: "identity-and-sign-in"
---

# Update identityProvider
Namespace: microsoft.graph

Update the properties of the specified identity provider configured in the tenant.

Among the types of providers derived from identityProviderBase, you can currently update a [socialIdentityProvider](../resources/socialidentityprovider.md) resource in Azure AD. In Azure AD B2C, this operation can currently update a [socialIdentityProvider](../resources/socialidentityprovider.md), or an [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) resource.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account)|IdentityProvider.ReadWrite.All|
|Delegated (personal Microsoft account)| Not supported.|
|Application| IdentityProvider.ReadWrite.All|

The work or school account needs to belong to one of the following roles:

* Global Administrator
* External Identity Provider Administrator

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/identityProviders/{id}
```

## Request headers

|Name|Description|
|:---------------|:----------|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body

In the request body, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD tenant.

In Azure AD B2C, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md), or an [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) object.

### socialIdentityProvider object

|Property|Type|Description|
|:---------------|:--------|:----------|
|clientId|String|The identifier for the client application obtained when registering the application with the identity provider.|
|clientSecret|String|The client secret for the application that is obtained when the application is registered with the identity provider. This is write-only. A read operation returns `****`.|
|displayName|String|The display name of the identity provider.|

### appleManagedIdentityProvider object

|Property|Type|Description|
|:---------------|:--------|:----------|
|displayName|String|The display name of the identity provider.|
|developerId|String|The Apple developer identifier.|
|serviceId|String|The Apple service identifier.|
|keyId|String|The Apple key identifier.|
|certificateData|String|The certificate data which is a long string of text from the certificate, can be null.|

## Response

If successful, this method returns a `204 No Content` response code. If unsuccessful, a `4xx` error will be returned with specific details.

## Examples

### Example 1: Update a specific **social identity provider** (Azure AD or Azure AD B2C)

#### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider",
  "sampleKeys": ["Amazon-OAUTH"]
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/identityProviders/Amazon-OAUTH
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.socialIdentityProvider",
  "clientSecret": "1111111111111"
}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-socialidentityprovider-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-socialidentityprovider-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-socialidentityprovider-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### Example 2: Update a specific **Apple identity provider** (only for Azure AD B2C)

#### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider",
  "sampleKeys": ["Apple-Managed-OIDC"]
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.socialIdentityProvider",
  "displayName": "Apple"
}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-appleidentityprovider-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-appleidentityprovider-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-appleidentityprovider-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
