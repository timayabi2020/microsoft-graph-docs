---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AllowedValue = {
	id : "Alpine",
	isActive : true,
};

const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitionsById("customSecurityAttributeDefinition-id").allowedValues.post(requestBody);
}


```