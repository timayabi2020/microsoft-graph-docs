---
title: "reportRoot: getAttackSimulationTrainingUserCoverage"
description: "List training coverage for users of a tenant in attack simulation and training campaigns."
author: "stuartcl"
ms.localizationpriority: medium
ms.prod: "reports"
doc_type: apiPageType
---

# reportRoot: getAttackSimulationTrainingUserCoverage (deprecated)
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

List [training coverage](../resources/attacksimulationtrainingusercoverage.md) for each user of a tenant in attack simulation and training campaigns.

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
GET /reports/getAttackSimulationTrainingUserCoverage
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [attackSimulationTrainingUserCoverage](../resources/attacksimulationtrainingusercoverage.md) collection in the response body.

## Examples

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getattacksimulationtrainingusercoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAttackSimulationTrainingUserCoverage
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/reportroot-getattacksimulationtrainingusercoverage-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attackSimulationTrainingUserCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "userTrainings": [
        {
          "assignedDateTime": "2021-01-01T01:01:01.01Z",
          "completionDateTime": "2021-01-02T01:01:01.01Z",
          "trainingStatus": "Completed",
          "displayName": "Sample Training"
        }
      ],
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
[securityReportsRoot: getAttackSimulationTrainingUserCoverage](securityreportsroot-getattacksimulationtrainingusercoverage.md)
