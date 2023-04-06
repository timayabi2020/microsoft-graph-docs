---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Location": "https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')",
	}
};
const requestBody : B2cIdentityUserFlow = {
	id : "Customer",
	userFlowType : UserFlowType.SignUpOrSignIn,
	userFlowTypeVersion : 3,
	identityProviders : [
		{
			id : "Facebook-OAuth",
		},
	],
};

const result = async () => {
	await graphServiceClient.identity.b2cUserFlows.post(requestBody, configuration);
}


```