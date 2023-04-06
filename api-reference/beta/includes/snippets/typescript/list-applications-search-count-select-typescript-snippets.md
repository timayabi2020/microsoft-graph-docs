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
		search: "\"displayName:Web\"",
		count: true,
		select: ["appId","identifierUris","displayName","publisherDomain","signInAudience"],
	}
};

const result = async () => {
	await graphServiceClient.applications.get(configuration);
}


```