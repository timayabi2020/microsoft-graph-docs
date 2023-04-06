---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : $refDeleteRequestBody = {
	additionalData : {
		"@odata.id" : "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
	},
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").ownersById("directoryObject-id").$ref.delete(requestBody);
}


```