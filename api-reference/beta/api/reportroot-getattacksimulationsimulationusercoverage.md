---
title: "reportRoot: getAttackSimulationSimulationUserCoverage"
description: "List simulation coverage for users of a tenant in attack simulation and training campaigns."
author: "stuartcl"
ms.localizationpriority: medium
ms.prod: "reports"
doc_type: apiPageType
---

# reportRoot: getAttackSimulationSimulationUserCoverage (deprecated)
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get [simulation coverage](../resources/attacksimulationsimulationusercoverage.md) for users of a tenant in attack simulation and training campaigns.

This function supports `@odata.nextLink` for pagination.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | AttackSimulation.Read.All                   |
| Delegated (personal Microsoft account) | Not supported.                              |
| Application                            | AttackSimulation.Read.All                   |

## HTTP request
[!INCLUDE [attacksim-deprecate-queryurl-reportapi](../includes/attacksim-deprecate-queryurl-reportapi.md)]

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getAttackSimulationSimulationUserCoverage
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [attackSimulationSimulationUserCoverage](../resources/attacksimulationsimulationusercoverage.md) collection in the response body.

## Examples

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getattacksimulationsimulationusercoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAttackSimulationSimulationUserCoverage
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/reportroot-getattacksimulationsimulationusercoverage-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attackSimulationSimulationUserCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "simulationCount": 2,
      "latestSimulationDateTime": "2021-01-01T01:01:01.01Z",
      "clickCount": 1,
      "compromisedCount": 1,
      "attackSimulationUser": {
        "userId": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      }
    }
  ]
}
```

## See also
[securityReportsRoot: getAttackSimulationSimulationUserCoverage](securityreportsroot-getattacksimulationsimulationusercoverage.md)

