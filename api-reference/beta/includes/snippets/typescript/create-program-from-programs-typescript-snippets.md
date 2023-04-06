---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Program = {
	displayName : "testprogram3",
	description : "test description",
};

const result = async () => {
	await graphServiceClient.programs.post(requestBody);
}


```