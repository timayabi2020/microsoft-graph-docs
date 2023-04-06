---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["id","category","displayName","description","version","executionConditions"],
	}
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.deletedItems.workflowsById("workflow-id").get(configuration);
}


```