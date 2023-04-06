---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SchemaExtension = {
	id : "courses",
	description : "Graph Learn training courses extensions",
	targetTypes : [
		"Group",
	],
	owner : "50897f70-a455-4adf-87bc-4cf17091d5ac",
	properties : [
		{
			name : "courseId",
			type : "Integer",
		},
		{
			name : "courseName",
			type : "String",
		},
		{
			name : "courseType",
			type : "String",
		},
	],
};

const result = async () => {
	await graphServiceClient.schemaExtensions.post(requestBody);
}


```