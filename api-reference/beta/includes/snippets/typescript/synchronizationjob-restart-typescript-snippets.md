---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Authorization": "Bearer <token>",
	}
};
const requestBody : RestartPostRequestBody = {
	criteria : {
		resetScope : SynchronizationJobRestartScope.Watermark, Escrows, QuarantineState,
	},
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").synchronization.jobsById("synchronizationJob-id").restart.post(requestBody, configuration);
}


```