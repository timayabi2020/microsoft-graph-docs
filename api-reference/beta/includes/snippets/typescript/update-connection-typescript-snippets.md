---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ExternalConnection = {
	name : "Contoso HR Service Tickets",
	description : "Connection to index HR service tickets",
};

const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").patch(requestBody);
}


```