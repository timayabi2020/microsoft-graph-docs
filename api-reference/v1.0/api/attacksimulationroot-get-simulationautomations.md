---
title: "Get simulationAutomation"
description: "Get an attack simulation automation for a tenant."
author: "stuartcl"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# Get simulationAutomation
Namespace: microsoft.graph

Get an attack simulation automation for a tenant.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | AttackSimulation.Read.All                   |
| Delegated (personal Microsoft account) | Not supported.                              |
| Application                            | AttackSimulation.Read.All                   |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}
```

## Optional query parameters
This method supports the `$count`, `$filter`, `$orderby`, `$skip`, `$top`, and `$select` [OData query parameters](/graph/query-parameters) to help customize the response. You can use the `$filter` and `$orderby` query parameters on the **displayName** and **status** properties.

If the result set spans multiple pages, the response body contains an `@odata.nextLink` that you can use to page through the result set.

The following are examples of their use:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}?$count=true
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}?$filter={property} eq '{property-value}'
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}?$filter={property} eq '{property-value}'&$top=5
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}?$orderby={property}
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}?$skip={skipCount}
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}?$top=1
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}?$select={property}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [simulationAutomation](../resources/simulationautomation.md) object in the response body.

## Examples

### Request

The following is an example of a request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_simulationautomation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/attackSimulation/simulationAutomations/fbad62b0-b32d-b6ac-9f48-d84bbea08f96
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-simulationautomation-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-simulationautomation-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-simulationautomation-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

The following is an example of the response.

>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.simulationAutomation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.simulationAutomation",
    "id": "fbad62b0-b32d-b6ac-9f48-d84bbea08f96",
    "displayName": "Reed Flores",
    "description": "Sample Simulation Automation Description",
    "status": "running",
    "createdDateTime": "2022-01-01T01:01:01.01Z",
    "createdBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Reed Flores",
        "email": "reed@contoso.com"
    },
    "lastModifiedDateTime": "2022-01-01T01:01:01.01Z",
    "lastModifiedBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Reed Flores",
        "email": "reed@contoso.com"
    },
    "lastRunDateTime": "2022-01-01T01:01:01.01Z",
    "nextRunDateTime": "2022-01-01T01:01:01.01Z"
}
```

