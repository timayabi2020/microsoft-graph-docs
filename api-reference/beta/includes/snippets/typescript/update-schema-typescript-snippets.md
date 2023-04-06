---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Schema = {
	baseType : "microsoft.graph.externalItem",
	properties : [
		{
			name : "ticketTitle",
			type : PropertyType.String,
			isSearchable : true,
			isRetrievable : true,
			labels : [
				label : Label.Title,
			],
		},
		{
			name : "priority",
			type : PropertyType.String,
			isQueryable : true,
			isRetrievable : true,
			isSearchable : false,
		},
		{
			name : "assignee",
			type : PropertyType.String,
			isRetrievable : true,
		},
	],
};

const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").schema.patch(requestBody);
}


```