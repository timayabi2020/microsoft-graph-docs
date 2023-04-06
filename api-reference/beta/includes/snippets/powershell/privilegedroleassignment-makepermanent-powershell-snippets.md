---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	reason = "reason-value"
	ticketNumber = "ticketNumber-value"
	ticketSystem = "ticketSystem-value"
}

New-MgBetaPrivilegedRoleAssignmentPermanent -PrivilegedRoleAssignmentId $privilegedRoleAssignmentId -BodyParameter $params

```