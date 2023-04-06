---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	approvalState = "approvalState-value"
	approverReason = "approverReason-value"
}

Update-MgBetaPrivilegedApproval -PrivilegedApprovalId $privilegedApprovalId -BodyParameter $params

```