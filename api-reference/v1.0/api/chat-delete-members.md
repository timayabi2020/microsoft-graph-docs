---
title: "Remove member from chat"
description: "Remove a conversationMember from a chat."
author: "AkJo"
ms.localizationpriority: high
ms.prod: "microsoft-teams"
doc_type: apiPageType
---

# Remove member from chat
Namespace: microsoft.graph

Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)| ChatMember.ReadWrite |
|Delegated (personal Microsoft account) | Not supported.    |
|Application| ChatMember.ReadWrite.All |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat",
  "sampleKeys": ["19:cf66807577b149cca1b7af0c32eec122@thread.v2", "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw=="]
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-members-from-chat-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/delete-members-from-chat-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/delete-members-from-chat-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### Response
The following is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## See also

- [Remove member from channel](channel-delete-members.md)
- [Remove member from team](team-delete-members.md)

