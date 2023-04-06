---
title: "Get softwareOathAuthenticationMethodConfiguration"
description: "Read the properties and relationships of a softwareOathAuthenticationMethodConfiguration object."
author: "jpettere"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Get softwareOathAuthenticationMethodConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [softwareOathAuthenticationMethodConfiguration](../resources/softwareoathauthenticationmethodconfiguration.md) object, which represents the third-party software OATH authentication method policy for the Azure AD tenant.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|Policy.Read.All, Policy.ReadWrite.AuthenticationMethod|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Policy.Read.All, Policy.ReadWrite.AuthenticationMethod|

For delegated scenarios, the administrator needs one of the following [Azure AD roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Global Reader
* Authentication Policy Administrator
* Global Administrator

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/softwareOath
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [softwareOathAuthenticationMethodConfiguration](../resources/softwareoathauthenticationmethodconfiguration.md) object in the response body.

## Examples

### Request
The following is an example of a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_softwareoathauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/softwareOath
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-softwareoathauthenticationmethodconfiguration-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-softwareoathauthenticationmethodconfiguration-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.softwareOathAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareOathAuthenticationMethodConfiguration",
    "id": "SoftwareOath",
    "state": "enabled",
    "includeTargets": [
      {
          "targetType": "group",
          "id": "all_users",
          "isRegistrationRequired": false
      }
    ],
    "excludeTargets": []
  }
}
```

