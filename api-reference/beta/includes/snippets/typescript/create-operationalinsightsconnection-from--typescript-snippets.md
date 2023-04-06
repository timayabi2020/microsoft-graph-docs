---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ResourceConnection = {
	"@odata.type" : "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
	additionalData : {
		"azureSubscriptionId" : "322ec614-e9c2-4cd5-a55c-5711fdecf02e",
		"azureResourceGroupName" : "target-resource-group",
		"workspaceName" : "my-workspace",
	},
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.resourceConnections.post(requestBody);
}


```