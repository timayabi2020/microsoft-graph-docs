---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Group = {
	displayName : "myGroup",
};

const result = async () => {
	await graphServiceClient.termStore.groups.post(requestBody);
}


```