---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CustomSecurityAttributeDefinition = {
	attributeSet : "Engineering",
	description : "Active projects for user",
	isCollection : true,
	isSearchable : true,
	name : "Project",
	status : "Available",
	type : "String",
	usePreDefinedValuesOnly : true,
};

const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitions.post(requestBody);
}


```