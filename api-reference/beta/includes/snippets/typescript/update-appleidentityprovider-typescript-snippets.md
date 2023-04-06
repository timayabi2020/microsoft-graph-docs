---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityProviderBase = {
	"@odata.type" : "#microsoft.graph.socialIdentityProvider",
	displayName : "Apple",
};

const result = async () => {
	await graphServiceClient.identity.identityProvidersById("identityProviderBase-id").patch(requestBody);
}


```