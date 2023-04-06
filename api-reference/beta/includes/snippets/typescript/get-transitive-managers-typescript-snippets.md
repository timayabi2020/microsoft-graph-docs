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
		expand: ["manager($levels=max;$select=id,displayName)"],
		select: ["id","displayName"],
		count: true,
	}
};

const result = async () => {
	await graphServiceClient.me.get(configuration);
}


```