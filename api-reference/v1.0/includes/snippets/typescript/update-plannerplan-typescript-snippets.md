---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "return=representation",
		"If-Match": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
	}
};
const requestBody : PlannerPlan = {
	title : "title-value",
};

const result = async () => {
	await graphServiceClient.planner.plansById("plannerPlan-id").patch(requestBody, configuration);
}


```