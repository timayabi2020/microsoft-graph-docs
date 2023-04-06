---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ProvisionOnDemandPostRequestBody = {
	parameters : [
		{
			ruleId : "6c409270-f78a-4bc6-af23-7cf3ab6482fe",
			subjects : [
				{
					objectId : "CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com",
					objectTypeName : "user",
				},
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").synchronization.jobsById("synchronizationJob-id").provisionOnDemand.post(requestBody);
}


```