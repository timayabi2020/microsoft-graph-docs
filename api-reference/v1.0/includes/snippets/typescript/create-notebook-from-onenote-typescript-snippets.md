---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Notebook = {
	displayName : "My Private notebook",
};

const result = async () => {
	await graphServiceClient.me.onenote.notebooks.post(requestBody);
}


```