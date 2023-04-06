---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityApiConnector = {
	displayName : "Test API",
	targetUrl : "https://someapi.com/api",
	authenticationConfiguration : {
		"@odata.type" : "#microsoft.graph.basicAuthentication",
		additionalData : {
			"username" : "<USERNAME>",
			"password" : "<PASSWORD>",
		},
	},
};

const result = async () => {
	await graphServiceClient.identity.apiConnectors.post(requestBody);
}


```