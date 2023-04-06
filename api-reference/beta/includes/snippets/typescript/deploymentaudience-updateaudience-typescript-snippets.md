---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UpdateAudiencePostRequestBody = {
	addMembers : [
		{
			"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
			id : "String (identifier)",
		},
	],
	removeMembers : [
		{
			"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
			id : "String (identifier)",
		},
	],
	addExclusions : [
		{
			"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
			id : "String (identifier)",
		},
	],
	removeExclusions : [
		{
			"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
			id : "String (identifier)",
		},
	],
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").audience.windowsUpdatesUpdateAudience.post(requestBody);
}


```