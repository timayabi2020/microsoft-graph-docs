---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UpdateAudienceByIdPostRequestBody = {
	memberEntityType : "String",
	addMembers : [
		"String",
	],
	removeMembers : [
		"String",
	],
	addExclusions : [
		"String",
	],
	removeExclusions : [
		"String",
	],
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").audience.windowsUpdatesUpdateAudienceById.post(requestBody);
}


```