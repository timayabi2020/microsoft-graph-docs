---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["category","displayName","versionNumber","executionConditions"],
		expand: ["tasks"],
	}
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflowsById("workflow-id").versionsById("workflowVersion-versionNumber").get(configuration);
}


```