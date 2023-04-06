---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	displayName = "Graph Simulation"
	payloadDeliveryPlatform = "email"
	"payload@odata.bind" = "https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a"
	durationInDays = 7
	attackTechnique = "credentialHarvesting"
	attackType = "social"
	status = "scheduled"
	completionDateTime = [System.DateTime]::Parse("2022-09-16T06:13:08.4297612Z")
	launchDateTime = [System.DateTime]::Parse("2022-09-05T06:13:08.4297612Z")
	includedAccountTarget = @{
		"@odata.type" = "#microsoft.graph.addressBookAccountTargetContent"
		type = "addressBook"
		accountTargetEmails = @(
			"john@contoso.com"
		)
	}
}

New-MgBetaSecurityAttackSimulation -BodyParameter $params

```