---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ProvisionOnDemandPostRequestBody = {
	parameters : [
		{
			ruleId : "33f7c90d-bf71-41b1-bda6-aaf0ddbee5d8#V2",
			subjects : [
				{
					objectId : "8213fd99-d6b6-417b-8e13-af6334856215",
					objectTypeName : "Group",
					links : {
						members : [
							{
								objectId : "cbc86211-6ada-4803-b73f-8039cf56d8a2",
								objectTypeName : "User",
							},
							{
								objectId : "2bc86211-6ada-4803-b73f-8039cf56d8a2",
								objectTypeName : "User",
							},
						],
					},
				},
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").synchronization.jobsById("synchronizationJob-id").provisionOnDemand.post(requestBody);
}


```