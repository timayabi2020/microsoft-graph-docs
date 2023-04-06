---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : QueryPostRequestBody = {
	requests : [
		{
			entityTypes : [
				entityType : EntityType.ChatMessage,
			],
			query : {
				queryString : "contoso from:bob to:alice sent>2022-07-14",
			},
			from : 0,
			size : 15,
			enableTopResults : true,
		},
	],
};

const result = async () => {
	await graphServiceClient.search.query.post(requestBody);
}


```