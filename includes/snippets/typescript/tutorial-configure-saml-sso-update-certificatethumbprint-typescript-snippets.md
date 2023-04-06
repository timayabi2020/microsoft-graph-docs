---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ServicePrincipal = {
	preferredTokenSigningKeyThumbprint : "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10",
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").patch(requestBody);
}


```