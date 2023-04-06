---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	appliesToCombinations = @(
		"fido2"
	)
}

Update-MgBetaIdentityConditionalAccessAuthenticationStrengthPolicyCombinationConfiguration -AuthenticationStrengthPolicyId $authenticationStrengthPolicyId -AuthenticationCombinationConfigurationId $authenticationCombinationConfigurationId -BodyParameter $params

```