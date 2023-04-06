---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Deployment = {
	"@odata.type" : "#microsoft.graph.windowsUpdates.deployment",
	state : {
		"@odata.type" : "microsoft.graph.windowsUpdates.deploymentState",
		requestedValue : RequestedDeploymentStateValue.Paused,
	},
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").patch(requestBody);
}


```