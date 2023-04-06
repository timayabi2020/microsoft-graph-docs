---
title: "Get authenticationStrengthPolicy"
description: "Read the properties and relationships of an authenticationStrengthPolicy object."
author: "mmcla"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Get authenticationStrengthPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [authenticationStrengthPolicy](../resources/authenticationstrengthpolicy.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|Policy.Read.All, Policy.ReadWrite.ConditionalAccess, Policy.ReadWrite.AuthenticationMethod|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Policy.Read.All, Policy.ReadWrite.ConditionalAccess, Policy.ReadWrite.AuthenticationMethod|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationStrengthPolicies/{authenticationStrengthPolicyId}
```

## Optional query parameters
This method does not support OData query parameters.

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [authenticationStrengthPolicy](../resources/authenticationstrengthpolicy.md) object in the response body.

## Examples

### Request
The following is an example of a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationstrengthpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationStrengthPolicies/00000000-0000-0000-0000-000000000004
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-authenticationstrengthpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-authenticationstrengthpolicy-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationStrengthPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type" : "#microsoft.graph.authenticationStrengthPolicy",
  "id": "00000000-0000-0000-0000-000000000004",
  "createdDateTime": "2017-10-30T10:59:01Z",
  "modifiedDateTime": "2017-10-30T10:59:01Z",
  "displayName": "Phishing resistant MFA",
  "description": "Phishing-resistant, Passwordless methods for the strongest authentication, such as a FIDO2 security key",
  "policyType": "builtIn",
  "requirementsSatisfied": "mfa",
  "allowedCombinations": [
      "windowsHelloForBusiness",
      "fido2",
      "x509CertificateMultiFactor"
  ],
  "combinationConfigurations": []
}
```

