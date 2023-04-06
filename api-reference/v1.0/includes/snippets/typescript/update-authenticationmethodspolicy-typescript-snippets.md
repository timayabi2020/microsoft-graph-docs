---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthenticationMethodsPolicy = {
	registrationEnforcement : {
		authenticationMethodsRegistrationCampaign : {
			snoozeDurationInDays : 1,
			state : AdvancedConfigState.Enabled,
			excludeTargets : [
			],
			includeTargets : [
				{
					id : "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
					targetType : AuthenticationMethodTargetType.Group,
					targetedAuthenticationMethod : "microsoftAuthenticator",
				},
			],
		},
	},
	authenticationMethodConfigurations : [
		{
			"@odata.type" : "#microsoft.graph.fido2AuthenticationMethodConfiguration",
			id : "Fido2",
			state : AuthenticationMethodState.Disabled,
			additionalData : {
				isSelfServiceRegistrationAllowed : false,
				isAttestationEnforced : false,
				keyRestrictions : {
					isEnforced : false,
					enforcementType : "block",
					aaGuids : [
					],
				},
			},
		},
	],
	additionalData : {
		"@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy",
	},
};

const result = async () => {
	await graphServiceClient.policies.authenticationMethodsPolicy.patch(requestBody);
}


```