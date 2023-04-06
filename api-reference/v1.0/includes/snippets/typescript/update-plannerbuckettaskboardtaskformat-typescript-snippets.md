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
const requestBody : PlannerBucketTaskBoardTaskFormat = {
	orderHint : "A6673H Ejkl!",
};

const result = async () => {
	await graphServiceClient.planner.tasksById("plannerTask-id").bucketTaskBoardFormat.patch(requestBody, configuration);
}


```