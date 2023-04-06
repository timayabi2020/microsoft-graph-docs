---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "name eq 'Project' and status eq 'Available'",
	}
};

const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitions.get(configuration);
}


```