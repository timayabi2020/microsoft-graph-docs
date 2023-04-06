---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	destinationId = "destinationId-value"
}

# A UPN can also be used as -UserId.
Move-MgUsersMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```