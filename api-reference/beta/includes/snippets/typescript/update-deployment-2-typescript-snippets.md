---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Deployment = {
	"@odata.type" : "#microsoft.graph.windowsUpdates.deployment",
	settings : {
		"@odata.type" : "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
		monitoring : {
			monitoringRules : [
				{
					signal : MonitoringSignal.Rollback,
					threshold : 5,
					action : MonitoringAction.PauseDeployment,
				},
			],
		},
	},
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.deploymentsById("deployment-id").patch(requestBody);
}


```