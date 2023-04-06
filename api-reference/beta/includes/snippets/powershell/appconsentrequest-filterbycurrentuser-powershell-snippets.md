---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Identity.Governance

Get-MgBetaIdentityGovernanceAppConsentRequest -AppConsentRequestId $appConsentRequestId -Filter "userConsentRequests/any(u:u/status eq 'InProgress')" 

```