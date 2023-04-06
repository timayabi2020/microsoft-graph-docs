---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ExternalGroup = {
	id : "31bea3d537902000",
	displayName : "Contoso Marketing",
	description : "The product marketing team",
};

const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").groups.post(requestBody);
}


```