---
title: "Update continuousAccessEvaluationPolicy"
description: "Update the properties of a continuousAccessEvaluationPolicy object."
author: "jerrysai"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Update continuousAccessEvaluationPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type                        | Permissions (from least to most privileged)                    |
|:--------------------------------------|:---------------------------------------------------------------|
|Delegated (work or school account)     | Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All |
|Delegated (personal Microsoft account) | Not supported. |
|Application                            | Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All |

> [!NOTE]
> This API has a [known issue](/graph/known-issues#permissions) related to permissions.  

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, don't include existing values that haven't changed.

|Property|Type|Description|
|:---|:---|:---|
|migrate|Boolean| `true` to indicate that the continuous access evaluation policy settings should be or has been migrated to the conditional access policy. |

## Response

If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.

## Examples

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_continuousaccessevaluationpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "migrate": true
}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-continuousaccessevaluationpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/update-continuousaccessevaluationpolicy-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```
