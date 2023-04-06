---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Term = {
	labels : [
		{
			name : "changedLabel",
			languageTag : "en-US",
			isDefault : true,
		},
	],
};

const result = async () => {
	await graphServiceClient.termStore.setsById("set-id").termsById("term-id").patch(requestBody);
}


```