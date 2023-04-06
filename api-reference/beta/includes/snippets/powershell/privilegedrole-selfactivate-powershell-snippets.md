---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	reason = "reason-value"
	duration = "duration-value"
	ticketNumber = "ticketNumber-value"
	ticketSystem = "ticketSystem-value"
}

Invoke-MgBetaSelfPrivilegedRoleActivate -PrivilegedRoleId $privilegedRoleId -BodyParameter $params

```