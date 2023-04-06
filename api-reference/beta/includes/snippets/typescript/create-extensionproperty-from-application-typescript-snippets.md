---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ExtensionProperty = {
	name : "jobGroup",
	dataType : "String",
	targetObjects : [
		"User",
	],
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").extensionProperties.post(requestBody);
}


```