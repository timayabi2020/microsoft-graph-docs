---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ActivatePostRequestBody = {
	subjects : [
		{
			id : "8cdf25a8-c9d2-423e-a03d-3f39f03c3e97",
		},
		{
			id : "ea09ac2e-77e3-4134-85f2-25ccf3c33387",
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflowsById("workflow-id").identityGovernanceActivate.post(requestBody);
}


```