---
title: "serviceHealthIssue: incidentReport"
description: "Provide the Post-Incident Review (PIR) document of a specified service issue for tenant."
author: "payiAzure"
ms.localizationpriority: medium
ms.prod: "service-communications"
doc_type: apiPageType
---

# serviceHealthIssue: incidentReport
Namespace: microsoft.graph

Provide the Post-Incident Review (PIR) document of a specified service issue for tenant. 

An issue only with status of `PostIncidentReviewPublished` indicates that the PIR document exists for the issue. The operation returns an error if the specified issue doesn't exist for the tenant or if PIR document does not exist for the issue.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|ServiceHealth.Read.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|ServiceHealth.Read.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}/incidentReport
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a file stream in the response body.

## Example

### Request


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO248163"],
  "name": "servicehealthissue_incidentreport"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/admin/serviceAnnouncement/issues/MO248163/incidentReport
```

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/servicehealthissue-incidentreport-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/servicehealthissue-incidentreport-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": "Stream"
}
```

