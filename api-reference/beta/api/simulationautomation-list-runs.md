---
title: "List runs"
description: "Get a list of the attack simulation automation runs for a tenant."
author: "Gopal-MSFT"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# List runs
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the attack simulation automation runs for a tenant.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | SecurityEvents.Read.All                     |
| Delegated (personal Microsoft account) | Not supported.                              |
| Application                            | SecurityEvents.Read.All                     |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}/runs
```

## Optional query parameters
This method supports the `$count`, `$skiptoken`, `$top`, and `$select` [OData query parameters](/graph/query-parameters) to help customize the response.

If the result set spans multiple pages, the response body contains an `@odata.nextLink` that you can use to page through the result set.

The following are examples of their use:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$count=true
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$skipToken={skipToken}
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$top=1
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$select={property}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [simulationAutomationRun](../resources/simulationautomationrun.md) objects in the response body.

## Examples

### Request

The following is an example of a request.

<!-- {
  "blockType": "request",
  "name": "list_simulationautomationrun"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulationAutomations/fbad62b0-b32d-b6ac-9f48-d84bbea08f96/runs
```


### Response

The following is an example of the response.

>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.simulationAutomationRun",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.simulationAutomationRun",
      "id": "ac4936a5-3865-a0ec-7254-67a22f6121e2",
      "status": "succeeded",
      "startDateTime": "2021-01-01T02:01:01.01Z",
      "endDateTime": "2021-01-01T02:01:01.01Z",
      "simulationId": "bc4936a5-3865-a0ec-7254-67a22f6121e2"
    }
  ]
}
```
