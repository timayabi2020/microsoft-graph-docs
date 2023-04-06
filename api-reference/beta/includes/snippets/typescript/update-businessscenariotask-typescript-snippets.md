---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BusinessScenarioTask = {
	"@odata.type" : "#microsoft.graph.businessScenarioTask",
	title : "Customer order #12010",
	percentComplete : 20,
	priority : 1,
	businessScenarioProperties : {
		externalObjectVersion : "000003",
	},
};

const result = async () => {
	await graphServiceClient.solutions.businessScenariosById("businessScenario-id").planner.tasksById("businessScenarioTask-id").patch(requestBody);
}


```