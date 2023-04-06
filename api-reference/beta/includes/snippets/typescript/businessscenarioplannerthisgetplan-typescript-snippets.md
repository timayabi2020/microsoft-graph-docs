---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GetPlanPostRequestBody = {
	target : {
		"@odata.type" : "microsoft.graph.businessScenarioGroupTarget",
		taskTargetKind : PlannerTaskTargetKind.Group,
		additionalData : {
			"groupId" : "7a339254-4b2b-4410-b295-c890a16776ee",
		},
	},
};

const result = async () => {
	await graphServiceClient.solutions.businessScenariosById("businessScenario-id").planner.getPlan.post(requestBody);
}


```