---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConfirmCompromisedPostRequestBody = {
	servicePrincipalIds : [
		"9089a539-a539-9089-39a5-899039a58990",
	],
};

const result = async () => {
	await graphServiceClient.identityProtection.riskyServicePrincipals.confirmCompromised.post(requestBody);
}


```