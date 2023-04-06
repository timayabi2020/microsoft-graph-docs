---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"OData-Version": "4.01",
	}
};
const requestBody : CustomSecurityAttributeDefinition = {
	additionalData : {
		allowedValues@delta : [
			{
				id : "Baker",
				isActive : false,
			},
			{
				id : "Skagit",
				isActive : true,
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitionsById("customSecurityAttributeDefinition-id").patch(requestBody, configuration);
}


```