---
title: Get printServiceEndpoint
description: Retrieve the properties and relationships of a print service endpoint.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
---

# Get printServiceEndpoint

Namespace: microsoft.graph

Retrieve the properties and relationships of a print service endpoint.

> [!NOTE]
> In order to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.

## Permissions

One of the following permissions is required to call these APIs. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:------------------------------------|
| Delegated (work or school account)     | PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrinterShare.ReadBasic.All, PrintJob.Read.All, Printer.Read.All, PrinterShare.Read.All, PrintConnector.Read.All, PrintSettings.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, Printer.ReadWrite.All, PrinterShare.ReadWrite.All, PrintJob.ReadWrite.All, PrintConnector.ReadWrite.All, PrintSettings.ReadWrite.All, Printer.Create, PrintJob.Create |
| Delegated (personal Microsoft account) | Not supported.                      |
| Application                            | Not supported.                      |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /print/services/{printServiceId}/endpoints/{printServiceEndpointId}
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

If successful, this method returns a `200 OK` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.

## Examples

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services/{printServiceId}/endpoints/{printServiceEndpointId}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-printserviceendpoint-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/get-printserviceendpoint-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/get-printserviceendpoint-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

> **Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "id": "mpsdiscovery",
  "displayName": "Microsoft Universal Print Discovery Service",
  "uri": "https://discovery.print.microsoft.com"
}
```
