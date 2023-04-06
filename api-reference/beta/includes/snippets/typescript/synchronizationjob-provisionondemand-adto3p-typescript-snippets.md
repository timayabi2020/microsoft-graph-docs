---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ProvisionOnDemandPostRequestBody = {
	parameters : [
		{
			subjects : [
				{
					objectId : "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
					objectTypeName : "User",
				},
			],
			ruleId : "ea807875-5618-4f0a-9125-0b46a05298ca",
		},
	],
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").synchronization.jobsById("synchronizationJob-id").provisionOnDemand.post(requestBody);
}


```