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
		search: "\"displayName:Pr\"",
		select: ["displayName","id"],
	}
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").members.graphUser.get(configuration);
}


```