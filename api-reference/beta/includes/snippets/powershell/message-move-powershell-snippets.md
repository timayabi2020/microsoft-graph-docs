---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	destinationId = "deleteditems"
}

# A UPN can also be used as -UserId.
Move-MgBetaUsersMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```