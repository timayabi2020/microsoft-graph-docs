---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConditionalAccessPolicy = {
	displayName : "Access to EXO requires MFA",
	state : ConditionalAccessPolicyState.Enabled,
	conditions : {
		clientAppTypes : [
			conditionalAccessClientApp : ConditionalAccessClientApp.MobileAppsAndDesktopClients,
			conditionalAccessClientApp : ConditionalAccessClientApp.Browser,
		],
		applications : {
			includeApplications : [
				"00000002-0000-0ff1-ce00-000000000000",
			],
		},
		users : {
			includeGroups : [
				"ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba",
			],
		},
		locations : {
			includeLocations : [
				"All",
			],
			excludeLocations : [
				"AllTrusted",
			],
		},
	},
	grantControls : {
		operator : "OR",
		builtInControls : [
			conditionalAccessGrantControl : ConditionalAccessGrantControl.Mfa,
		],
	},
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.policies.post(requestBody);
}


```