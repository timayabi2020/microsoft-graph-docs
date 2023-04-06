---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CustomSecurityAttributeDefinition = {
	attributeSet : "Engineering",
	description : "Target completion date",
	isCollection : false,
	isSearchable : true,
	name : "ProjectDate",
	status : "Available",
	type : "String",
	usePreDefinedValuesOnly : false,
};

const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitions.post(requestBody);
}


```