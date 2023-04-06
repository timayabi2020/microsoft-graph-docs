---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "attributeSet eq 'Engineering' and status eq 'Available' and type eq 'String'",
	}
};

const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitions.get(configuration);
}


```