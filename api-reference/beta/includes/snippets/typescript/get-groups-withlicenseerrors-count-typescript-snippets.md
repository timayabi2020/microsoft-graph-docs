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
		filter: "hasMembersWithLicenseErrors eq true",
		select: ["id","displayName"],
	}
};

const result = async () => {
	await graphServiceClient.groups.get(configuration);
}


```