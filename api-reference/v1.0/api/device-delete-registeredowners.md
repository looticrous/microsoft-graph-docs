---
title: "Delete registeredOwners"
description: "Remove a user as a registered owner of the device."
localization_priority: Normal
author: "michaelrm97"
ms.prod: "microsoft-identity-platform"
doc_type: apiPageType
---

# Delete registeredOwner

Namespace: microsoft.graph

Remove a user as a registered owner of the device.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) |Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Directory.ReadWrite.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredOwners/{id}/$ref
```

## Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Example
##### Request
Here is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredowners"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners/{id}/$ref
```

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
  "description": "Delete registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->