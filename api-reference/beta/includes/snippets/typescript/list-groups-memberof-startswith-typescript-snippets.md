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
		count: true,
		orderby: ["displayName"],
		filter: "startswith(displayName,%20'A')",
	}
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").memberOf.graphGroup.get(configuration);
}


```