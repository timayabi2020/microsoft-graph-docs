---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SchemaPostRequestBody = {
	additionalData : {
		"baseType" : "microsoft.graph.externalItem",
		properties : [
			{
				name : "ticketTitle",
				type : "string",
				isSearchable : "true",
				isRetrievable : "true",
				labels : [
					"title",
				],
			},
			{
				name : "priority",
				type : "string",
				isQueryable : "true",
				isRetrievable : "true",
				isSearchable : "false",
			},
			{
				name : "assignee",
				type : "string",
				isRetrievable : "true",
			},
		],
	},
};

async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").schema.post(requestBody);
}


```