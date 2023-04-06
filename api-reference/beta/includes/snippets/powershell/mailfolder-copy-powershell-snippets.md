---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	destinationId = "destinationId-value"
}

# A UPN can also be used as -UserId.
Copy-MgBetaUsersMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```