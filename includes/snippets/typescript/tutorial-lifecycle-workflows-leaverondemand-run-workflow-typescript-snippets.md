---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ActivatePostRequestBody = {
	subjects : [
		{
			id : "8930f0c7-cdd7-4885-9260-3b4a8111de5c",
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflowsById("workflow-id").identityGovernanceActivate.post(requestBody);
}


```