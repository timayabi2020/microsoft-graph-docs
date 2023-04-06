---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"ConsistencyLevel": "eventual",
	}
,	queryParameters : {
		filter: "extensionAttributes/extensionAttribute1 eq 'BYOD-Device'",
		count: true,
	}
};

const result = async () => {
	await graphServiceClient.devices.get(configuration);
}


```