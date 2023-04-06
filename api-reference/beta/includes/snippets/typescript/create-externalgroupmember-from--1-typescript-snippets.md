---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Identity = {
	id : "e811976d-83df-4cbd-8b9b-5215b18aa874",
	type : IdentityType.User,
};

const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").groupsById("externalGroup-id").members.post(requestBody);
}


```