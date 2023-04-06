---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityApiConnector = {
	displayName : "New Test API",
	targetUrl : "https://otherapi.com/api/endpoint",
	authenticationConfiguration : {
		"@odata.type" : "microsoft.graph.basicAuthentication",
		additionalData : {
			"username" : "<NEW_USERNAME>",
			"password" : "<NEW_PASSWORD>",
		},
	},
};

const result = async () => {
	await graphServiceClient.identity.apiConnectorsById("identityApiConnector-id").patch(requestBody);
}


```