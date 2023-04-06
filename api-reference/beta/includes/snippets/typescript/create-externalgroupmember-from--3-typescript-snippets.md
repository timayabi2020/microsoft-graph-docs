---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Identity = {
	id : "1431b9c38ee647f6a",
	type : IdentityType.ExternalGroup,
};

const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").groupsById("externalGroup-id").members.post(requestBody);
}


```