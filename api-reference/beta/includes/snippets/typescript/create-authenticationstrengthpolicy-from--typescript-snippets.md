---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthenticationStrengthPolicy = {
	"@odata.type" : "#microsoft.graph.authenticationStrengthPolicy",
	displayName : "Contoso authentication level",
	description : "The only authentication level allowed to access our secret apps",
	allowedCombinations : [
		authenticationMethodModes : AuthenticationMethodModes.Password, hardwareOath,
		authenticationMethodModes : AuthenticationMethodModes.Password, sms,
	],
};

const result = async () => {
	await graphServiceClient.policies.authenticationStrengthPolicies.post(requestBody);
}


```