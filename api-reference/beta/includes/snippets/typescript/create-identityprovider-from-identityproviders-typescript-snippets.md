---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityProvider = {
	"@odata.type" : "microsoft.graph.identityProvider",
	name : "Login with Amazon",
	type : "Amazon",
	clientId : "56433757-cadd-4135-8431-2c9e3fd68ae8",
	clientSecret : "000000000000",
};

const result = async () => {
	await graphServiceClient.identityProviders.post(requestBody);
}


```