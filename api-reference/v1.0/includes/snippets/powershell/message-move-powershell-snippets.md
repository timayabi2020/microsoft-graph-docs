---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
	destinationId = "deleteditems"
}

# A UPN can also be used as -UserId.
Move-MgUsersMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```