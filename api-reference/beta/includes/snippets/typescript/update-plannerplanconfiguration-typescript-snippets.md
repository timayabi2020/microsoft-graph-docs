---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PlannerPlanConfiguration = {
	"@odata.type" : "#microsoft.graph.plannerPlanConfiguration",
	defaultLanguage : "en-us",
	buckets : [
		{
			externalBucketId : "deliveryBucket",
		},
		{
			externalBucketId : "storePickupBucket",
		},
		{
			externalBucketId : "specialOrdersBucket",
		},
		{
			externalBucketId : "returnProcessingBucket",
		},
	],
};

const result = async () => {
	await graphServiceClient.solutions.businessScenariosById("businessScenario-id").planner.planConfiguration.patch(requestBody);
}


```