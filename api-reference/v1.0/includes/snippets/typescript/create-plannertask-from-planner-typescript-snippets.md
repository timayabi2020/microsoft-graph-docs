---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PlannerTask = {
	planId : "xqQg5FS2LkCp935s-FIFm2QAFkHM",
	bucketId : "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
	title : "Update client list",
	assignments : {
		additionalData : {
			"fbab97d0-4932-4511-b675-204639209557" : {
				"@odata.type" : "#microsoft.graph.plannerAssignment",
				orderHint : " !",
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.planner.tasks.post(requestBody);
}


```