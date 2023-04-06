---
title: "List plannerPlanConfigurationLocalizations"
description: "Get a list of the plannerPlanConfigurationLocalization objects and their properties."
author: "TarkanSevilmis"
ms.localizationpriority: medium
ms.prod: "business-scenarios"
doc_type: apiPageType
---

# List plannerPlanConfigurationLocalizations

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [plannerPlanConfigurationLocalization](../resources/plannerplanconfigurationlocalization.md) objects and their properties.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|BusinessScenarioConfig.Read.OwnedBy, BusinessScenarioConfig.ReadWrite.OwnedBy, BusinessScenarioConfig.Read.All, BusinessScenarioConfig.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|BusinessScenarioConfig.Read.OwnedBy, BusinessScenarioConfig.ReadWrite.OwnedBy|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

For localizations based on a business scenario ID:

``` http
GET /solutions/businessScenarios/{businessScenarioId}/planner/planConfiguration/localizations
```

For localizations based on the unique name of a business scenario:

``` http
GET /solutions/businessScenarios(uniqueName='{uniqueName}')/planner/planConfiguration/localizations
```

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [plannerPlanConfigurationLocalization](../resources/plannerplanconfigurationlocalization.md) objects in the response body.

## Examples

### Example 1: Get all localizations

The following example shows a request that gets all localized names for a [plannerPlanConfiguration](../resources/plannerplanconfiguration.md).

#### Request

The following is an example of a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerplanconfigurationlocalization",
  "sampleKeys": ["c5d514e6c6864911ac46c720affb6e4d"]
}
-->
``` http
GET https://graph.microsoft.com/beta/solutions/businessScenarios/c5d514e6c6864911ac46c720affb6e4d/planner/planConfiguration/localizations
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-plannerplanconfigurationlocalization-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/list-plannerplanconfigurationlocalization-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### Response

The following is an example of the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.plannerPlanConfigurationLocalization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerPlanConfigurationLocalization",
      "id": "en-us",
      "languageTag": "en-us",
      "planTitle": "Order Tracking",
      "buckets": [
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "deliveryBucket",
              "name": "Deliveries"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "storePickupBucket",
              "name": "Pickup"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "specialOrdersBucket",
              "name": "Special Orders"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "returnProcessingBucket",
              "name": "Customer Returns"
          }
      ]
    },
    {
      "@odata.type": "#microsoft.graph.plannerPlanConfigurationLocalization",
      "id": "pt-br",
      "languageTag": "pt-br",
      "planTitle": "Acompanhamento de pedidos",
      "buckets": [
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "deliveryBucket",
              "name": "Entregas"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "storePickupBucket",
              "name": "Retirada na loja"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "specialOrdersBucket",
              "name": "Pedidos especiais"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "returnProcessingBucket",
              "name": "Devoluções"
          }
      ]
    }
  ]
}
```

### Example 2: Get localization for a specific language tag

The following example shows a request that gets all localized names for a [plannerPlanConfiguration](../resources/plannerplanconfiguration.md) for a specific language.

#### Request

The following is an example of a request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerplanconfigurationlocalization",
  "sampleKeys": ["c5d514e6c6864911ac46c720affb6e4d"]
}
-->
``` http
GET https://graph.microsoft.com/beta/solutions/businessScenarios/c5d514e6c6864911ac46c720affb6e4d/planner/planConfiguration/localizations?$filter=languageTag eq 'en-us'
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-plannerplanconfigurationlocalization-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/list-plannerplanconfigurationlocalization-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### Response

The following is an example of the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.plannerPlanConfigurationLocalization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerPlanConfigurationLocalization",
      "id": "en-us",
      "languageTag": "en-us",
      "planTitle": "Order Tracking",
      "buckets": [
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "deliveryBucket",
              "name": "Deliveries"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "storePickupBucket",
              "name": "Pickup"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "specialOrdersBucket",
              "name": "Special Orders"
          },
          {
              "@odata.type": "microsoft.graph.plannerPlanConfigurationBucketLocalization",
              "externalBucketId": "returnProcessingBucket",
              "name": "Customer Returns"
          }
      ]
    }
  ]
}
```
