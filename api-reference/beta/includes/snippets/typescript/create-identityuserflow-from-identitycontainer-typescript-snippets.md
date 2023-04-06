---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityUserFlow = {
	id : "Pol1",
	userFlowType : UserFlowType.SignUpOrSignIn,
	userFlowTypeVersion : 1,
};

const result = async () => {
	await graphServiceClient.identity.userFlows.post(requestBody);
}


```