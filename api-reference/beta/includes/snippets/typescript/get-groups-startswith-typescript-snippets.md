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
		filter: "startswith(displayName,%20'a')",
		count: true,
		top: 1,
		orderby: ["displayName"],
	}
};

const result = async () => {
	await graphServiceClient.groups.get(configuration);
}


```