---
title: "Update authorizationpolicy"
description: "Update the properties of authorizationPolicy object."
ms.localizationpriority: medium
author: "DougKirschner"
ms.prod: "identity-and-sign-in"
doc_type: "apiPageType"
---

# Update authorizationPolicy

Namespace: microsoft.graph

Update the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | Policy.ReadWrite.Authorization|
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | Policy.ReadWrite.Authorization|

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## Request headers

| Name       | Description|
|:-----------|:-----------|
| Authorization | Bearer {token}. Required. |
| Content-type | application/json. Required. |

## Request body

In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, don't include existing values that haven't changed.

| Property     | Type        | Description |
|:-------------|:------------|:------------|
|allowedToSignUpEmailBasedSubscriptions|Boolean| Indicates whether users can sign up for email based subscriptions. |
|allowedToUseSSPR|Boolean| Indicates whether the Self-Serve Password Reset feature can be used by users on the tenant. |
|allowEmailVerifiedUsersToJoinOrganization|Boolean| Indicates whether a user can join the tenant by email validation. |
|allowInvitesFrom|allowInvitesFrom|Indicates who can invite external users to the organization. Possible values are: `none`, `adminsAndGuestInviters`, `adminsGuestInvitersAndAllMembers`, `everyone`.  `everyone` is the default setting for all cloud environments except US Government. See more on the allowed values in this [table](../resources/authorizationpolicy.md#allowinvitesfrom-values). |
|blockMsolPowerShell|Boolean| To disable the use of MSOL PowerShell set this property to `true`. This will also disable user-based access to the legacy service endpoint used by MSOL PowerShell. This does not affect Azure AD Connect or Microsoft Graph. |
|defaultUserRolePermissions|[defaultUserRolePermissions](../resources/defaultuserrolepermissions.md)| Specifies certain customizable permissions for default user role. |
|description|String| Description of this policy.|
|displayName|String| Display name for this policy. |
|guestUserRoleId|Guid| Represents role templateId for the role that should be granted to guest user. Currently following roles are supported:  User (`a0b1b346-4d3e-4e8b-98f8-753987be4970`), Guest User (`10dae51f-b6af-4016-8d66-8c2a99b929b3`), and Restricted Guest User (`2af84b1e-32c8-42b7-82bc-daa82404023b`). |


## Response

If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.

## Examples

### Example 1: Update or set Guest user access level for the tenant

#### Request

The following is an example of the request. In this example, guest access level is modified to Restricted Guest User.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
  "allowEmailVerifiedUsersToJoinOrganization":false
}
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-authzpolicy-guestuserlevel-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-authzpolicy-guestuserlevel-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### Example 2: Block MSOL PowerShell in tenant

#### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-authzpolicy-blockmsolpowershell-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-authzpolicy-blockmsolpowershell-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### Example 3: Disable default user role's permission to create applications

#### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-authzpolicy-applications-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-authzpolicy-applications-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### Example 4: Enable default user role to use Self-Serve Password Reset feature

#### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-authzpolicy-sspr-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-authzpolicy-sspr-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### Example 5: Disable user consent to apps for default user role

#### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": []
   }
}
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-authzpolicy-disableuserconsent-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-authzpolicy-disableuserconsent-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### Example 6: Enable user consent to apps, subject to app consent policy

#### Request

The following is an example of the request that allows user consent to apps, subject to the built-in [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low`, which allows delegated permissions classified "low", for client apps from verified publishers or registered in the same tenant.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": [
         "managePermissionGrantsForSelf.microsoft-user-default-low"
      ]
   }
}
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-authzpolicy-enableuserconsentlow-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/update-authzpolicy-enableuserconsentlow-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### Response

The following is an example of the response.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
