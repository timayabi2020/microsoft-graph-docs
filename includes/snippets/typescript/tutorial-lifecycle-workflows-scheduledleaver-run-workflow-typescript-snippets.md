---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ActivatePostRequestBody = {
	subjects : [
		{
			id : "df744d9e-2148-4922-88a8-633896c1e929",
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflowsById("workflow-id").identityGovernanceActivate.post(requestBody);
}


```