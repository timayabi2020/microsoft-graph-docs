---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "category eq 'leaver'",
		select: ["id","category","displayName","isEnabled","isSchedulingEnabled"],
	}
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflows.get(configuration);
}


```