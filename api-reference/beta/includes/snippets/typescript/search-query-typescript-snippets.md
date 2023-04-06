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
				entityType : EntityType.ExternalItem,
			],
			contentSources : [
				"/external/connections/connectionfriendlyname",
			],
			query : {
				queryString : "contoso product",
			},
			from : 0,
			size : 25,
			fields : [
				"title",
				"description",
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.search.query.post(requestBody);
}


```