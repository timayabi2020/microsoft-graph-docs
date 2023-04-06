---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthenticationCombinationConfiguration = {
	"@odata.type" : "#microsoft.graph.fido2CombinationConfiguration",
	appliesToCombinations : [
		authenticationMethodModes : AuthenticationMethodModes.Fido2,
	],
	additionalData : {
		allowedAAGUIDs : [
			"486c3b50-889c-480a-abc5-c04ef7c873e0",
			"c042882f-a621-40c8-94d3-9cde3a826fed",
			"ec454c08-4c77-4012-9d48-45f7f0fccdfb",
		],
	},
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.authenticationStrengths.policiesById("authenticationStrengthPolicy-id").combinationConfigurations.post(requestBody);
}


```