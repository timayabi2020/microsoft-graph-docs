---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PlannerPlanConfigurationLocalization = {
	"@odata.type" : "#microsoft.graph.plannerPlanConfigurationLocalization",
	planTitle : "Order Tracking",
	buckets : [
		{
			externalBucketId : "deliveryBucket",
			name : "Deliveries",
		},
		{
			externalBucketId : "storePickupBucket",
			name : "Pickup",
		},
		{
			externalBucketId : "specialOrdersBucket",
			name : "Special Orders",
		},
		{
			externalBucketId : "returnProcessingBucket",
			name : "Customer Returns",
		},
	],
};

const result = async () => {
	await graphServiceClient.solutions.businessScenariosById("businessScenario-id").planner.planConfiguration.localizationsById("plannerPlanConfigurationLocalization-id").patch(requestBody);
}


```