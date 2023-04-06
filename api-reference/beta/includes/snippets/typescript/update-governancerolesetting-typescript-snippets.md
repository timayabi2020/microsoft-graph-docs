---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GovernanceRoleSetting = {
	adminEligibleSettings : [
		{
			ruleIdentifier : "ExpirationRule",
			setting : "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}",
		},
	],
};

const result = async () => {
	await graphServiceClient.privilegedAccessById("privilegedAccess-id").roleSettingsById("governanceRoleSetting-id").patch(requestBody);
}


```