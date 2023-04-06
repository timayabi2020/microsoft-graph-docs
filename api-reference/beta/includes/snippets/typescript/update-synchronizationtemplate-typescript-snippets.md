---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Authorization": "Bearer <token>",
	}
};
const requestBody : Template = {
	additionalData : {
		"id" : "Slack",
		"applicationId" : "{id}",
		"factoryTag" : "CustomSCIM",
	},
};

async () => {
	await graphServiceClient.applicationsById("application-id").synchronization.templatesById("synchronizationTemplate-id").put(requestBody, configuration);
}


```