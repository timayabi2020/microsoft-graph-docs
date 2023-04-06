---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConditionalAccessPolicy = {
	displayName : "Block access to EXO non-trusted regions.",
	state : ConditionalAccessPolicyState.Enabled,
	conditions : {
		clientAppTypes : [
			conditionalAccessClientApp : ConditionalAccessClientApp.All,
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
				"198ad66e-87b3-4157-85a3-8a7b51794ee9",
			],
		},
	},
	grantControls : {
		operator : "OR",
		builtInControls : [
			conditionalAccessGrantControl : ConditionalAccessGrantControl.Block,
		],
	},
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.policies.post(requestBody);
}


```