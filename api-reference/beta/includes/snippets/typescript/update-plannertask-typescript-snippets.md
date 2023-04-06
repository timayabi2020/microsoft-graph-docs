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
const requestBody : PlannerTask = {
	assignments : {
		additionalData : {
			"fbab97d0-4932-4511-b675-204639209557" : {
				"@odata.type" : "#microsoft.graph.plannerAssignment",
				orderHint : "N9917 U2883!",
			},
		},
	},
	appliedCategories : {
		additionalData : {
			category3 : true,
			category4 : false,
		},
	},
};

const result = async () => {
	await graphServiceClient.planner.tasksById("plannerTask-id").patch(requestBody, configuration);
}


```