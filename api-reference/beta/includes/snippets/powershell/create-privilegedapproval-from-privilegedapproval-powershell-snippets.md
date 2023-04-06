---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	userId = "userId-value"
	roleId = "roleId-value"
	approvalType = "approvalType-value"
	approvalState = "approvalState-value"
	approvalDuration = "datetime-value"
}

New-MgBetaPrivilegedApproval -BodyParameter $params

```