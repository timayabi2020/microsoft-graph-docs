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
const requestBody : PlannerPlanDetails = {
	sharedWith : {
		additionalData : {
			"6463a5ce-2119-4198-9f2a-628761df4a62" : true,
			"d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
		},
	},
	categoryDescriptions : {
		category1 : "Indoors",
		category3 : null,
	},
};

const result = async () => {
	await graphServiceClient.planner.plansById("plannerPlan-id").details.patch(requestBody, configuration);
}


```