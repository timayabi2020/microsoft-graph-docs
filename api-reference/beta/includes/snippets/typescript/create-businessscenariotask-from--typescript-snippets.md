---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BusinessScenarioTask = {
	"@odata.type" : "#microsoft.graph.businessScenarioTask",
	title : "Customer order #12010",
	percentComplete : 0,
	priority : 5,
	target : {
		"@odata.type" : "microsoft.graph.businessScenarioGroupTarget",
		taskTargetKind : PlannerTaskTargetKind.Group,
		additionalData : {
			"groupId" : "7a339254-4b2b-4410-b295-c890a16776ee",
		},
	},
	businessScenarioProperties : {
		externalObjectId : "Order#12010",
		externalContextId : "Warehouse-CA-36",
		externalObjectVersion : "000001",
		webUrl : "https://ordertracking.contoso.com/view?id=12010",
		externalBucketId : "deliveryBucket",
	},
};

const result = async () => {
	await graphServiceClient.solutions.businessScenariosById("businessScenario-id").planner.tasks.post(requestBody);
}


```