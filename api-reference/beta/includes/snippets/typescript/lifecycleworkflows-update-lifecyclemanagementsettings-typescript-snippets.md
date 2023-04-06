---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : LifecycleManagementSettings = {
	workflowScheduleIntervalInHours : 3,
	additionalData : {
		"@odata.context" : "https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.settings.patch(requestBody);
}


```