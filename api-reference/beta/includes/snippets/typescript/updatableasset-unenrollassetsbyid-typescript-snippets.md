---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnenrollAssetsByIdPostRequestBody = {
	updateCategory : UpdateCategory.Feature,
	memberEntityType : "#microsoft.graph.windowsUpdates.azureADDevice",
	ids : [
		"String",
		"String",
		"String",
	],
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.updatableAssets.windowsUpdatesUnenrollAssetsById.post(requestBody);
}


```