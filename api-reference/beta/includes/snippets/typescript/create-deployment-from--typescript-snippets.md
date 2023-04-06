---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Deployment = {
	"@odata.type" : "#microsoft.graph.windowsUpdates.deployment",
	content : {
		"@odata.type" : "microsoft.graph.windowsUpdates.featureUpdateReference",
		additionalData : {
			"version" : "20H2",
		},
	},
	settings : {
		"@odata.type" : "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
		monitoring : {
			monitoringRules : [
				{
					"@odata.type" : "#microsoft.graph.windowsUpdates.monitoringRule",
					signal : MonitoringSignal.Rollback,
					threshold : 5,
					action : MonitoringAction.PauseDeployment,
				},
			],
		},
		additionalData : {
			rollout : {
				devicesPerOffer : 100,
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.admin.windows.updates.deployments.post(requestBody);
}


```