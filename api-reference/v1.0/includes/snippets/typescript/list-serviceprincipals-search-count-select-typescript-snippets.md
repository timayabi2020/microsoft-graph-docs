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
		search: "\"displayName:Team\"",
		count: true,
		select: ["accountEnabled","displayName","publisherName","servicePrincipalType","signInAudience"],
	}
};

const result = async () => {
	await graphServiceClient.servicePrincipals.get(configuration);
}


```