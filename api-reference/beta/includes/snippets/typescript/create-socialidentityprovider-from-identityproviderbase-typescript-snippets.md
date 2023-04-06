---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityProviderBase = {
	"@odata.type" : "microsoft.graph.socialIdentityProvider",
	displayName : "Login with Amazon",
	additionalData : {
		"identityProviderType" : "Amazon",
		"clientId" : "56433757-cadd-4135-8431-2c9e3fd68ae8",
		"clientSecret" : "000000000000",
	},
};

const result = async () => {
	await graphServiceClient.identity.identityProviders.post(requestBody);
}


```