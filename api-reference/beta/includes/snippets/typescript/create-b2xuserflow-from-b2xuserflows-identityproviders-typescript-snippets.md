---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : B2xIdentityUserFlow = {
	id : "Partner",
	userFlowType : UserFlowType.SignUpOrSignIn,
	userFlowTypeVersion : 1,
	identityProviders : [
		{
			id : "Facebook-OAuth",
			type : "Facebook",
			name : "Facebook",
		},
	],
};

const result = async () => {
	await graphServiceClient.identity.b2xUserFlows.post(requestBody);
}


```