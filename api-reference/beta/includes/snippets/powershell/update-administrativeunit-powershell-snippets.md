---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	membershipType = "Dynamic"
	membershipRule = "(user.country -eq "United States")"
	membershipRuleProcessingState = "On"
}

Update-MgBetaAdministrativeUnit -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```