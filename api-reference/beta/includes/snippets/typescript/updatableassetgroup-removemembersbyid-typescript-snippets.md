---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RemoveMembersByIdPostRequestBody = {
	ids : [
		"String",
		"String",
		"String",
	],
	memberEntityType : "#microsoft.graph.windowsUpdates.azureADDevice",
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.updatableAssetsById("updatableAsset-id").windowsUpdatesRemoveMembersById.post(requestBody);
}


```