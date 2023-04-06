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
		filter: "owners/$count eq 0 or owners/$count eq 1",
		count: true,
		select: ["id","displayName"],
	}
};

const result = async () => {
	await graphServiceClient.servicePrincipals.get(configuration);
}


```