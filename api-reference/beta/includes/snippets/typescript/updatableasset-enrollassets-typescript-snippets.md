---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EnrollAssetsPostRequestBody = {
	updateCategory : UpdateCategory.String,
	assets : [
		{
			"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
			id : "String (identifier)",
		},
	],
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.updatableAssets.windowsUpdatesEnrollAssets.post(requestBody);
}


```