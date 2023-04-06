---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Workflow = {
	description : "Configure new hire tasks for onboarding employees on their first day",
	displayName : "Australia Onboard new hire employee",
	isEnabled : true,
	isSchedulingEnabled : false,
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflowsById("workflow-id").patch(requestBody);
}


```