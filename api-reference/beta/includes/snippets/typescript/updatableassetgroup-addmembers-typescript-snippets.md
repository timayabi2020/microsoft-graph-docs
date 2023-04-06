---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddMembersPostRequestBody = {
	assets : [
		{
			"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice",
			id : "String (identifier)",
		},
	],
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.updatableAssetsById("updatableAsset-id").windowsUpdatesAddMembers.post(requestBody);
}


```