---
title: "Delete event"
description: "Delete event."
author: "iamgirishck"
ms.localizationpriority: medium
ms.prod: "outlook"
doc_type: apiPageType
---

# Delete event

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Removes the specified [event](../resources/event.md) from the containing calendar. 

If the event is a meeting, deleting the event on the organizer's calendar sends a cancellation message to the meeting attendees.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Calendars.ReadWrite    |
|Delegated (personal Microsoft account) | Calendars.ReadWrite    |
|Application | Calendars.ReadWrite |

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns `204 No Content` response code. It does not return anything in the response body.

## Example
##### Request
Here is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-event-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/delete-event-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### Response

Here is an example of the response. 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


