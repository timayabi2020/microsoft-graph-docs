---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConditionalAccessPolicy = {
	displayName : "Policy for risky sign-in",
	state : ConditionalAccessPolicyState.Enabled,
	conditions : {
		signInRiskLevels : [
			riskLevel : RiskLevel.High,
			riskLevel : RiskLevel.Medium,
		],
		applications : {
			includeApplications : [
				"All",
			],
		},
		users : {
			includeUsers : [
				"4628e7df-dff3-407c-a08f-75f08c0806dc",
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