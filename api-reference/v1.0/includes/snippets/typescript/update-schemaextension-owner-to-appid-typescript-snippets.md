---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SchemaExtension = {
	owner : "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa",
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
		{
			name : "courseSupervisors",
			type : "String",
		},
	],
};

const result = async () => {
	await graphServiceClient.schemaExtensionsById("schemaExtension-id").patch(requestBody);
}


```