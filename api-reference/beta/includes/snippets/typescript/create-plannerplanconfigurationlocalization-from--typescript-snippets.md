---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PlannerPlanConfigurationLocalization = {
	"@odata.type" : "#microsoft.graph.plannerPlanConfigurationLocalization",
	languageTag : "en-us",
	planTitle : "Order Tracking",
	buckets : [
		{
			"@odata.type" : "microsoft.graph.plannerPlanConfigurationBucketLocalization",
			externalBucketId : "deliveryBucket",
			name : "Deliveries",
		},
		{
			"@odata.type" : "microsoft.graph.plannerPlanConfigurationBucketLocalization",
			externalBucketId : "storePickupBucket",
			name : "Pickup",
		},
		{
			"@odata.type" : "microsoft.graph.plannerPlanConfigurationBucketLocalization",
			externalBucketId : "specialOrdersBucket",
			name : "Special Orders",
		},
		{
			"@odata.type" : "microsoft.graph.plannerPlanConfigurationBucketLocalization",
			externalBucketId : "returnProcessingBucket",
			name : "Customer Returns",
		},
	],
};

const result = async () => {
	await graphServiceClient.solutions.businessScenariosById("businessScenario-id").planner.planConfiguration.localizations.post(requestBody);
}


```