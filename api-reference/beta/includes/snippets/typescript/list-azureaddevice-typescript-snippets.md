---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "isof('microsoft.graph.windowsUpdates.azureADDevice')",
	}
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.updatableAssets.get(configuration);
}


```