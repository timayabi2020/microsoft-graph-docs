---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewStage = {
	"@odata.type" : "#microsoft.graph.accessReviewStage",
	reviewers : [
		{
			query : "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
			queryType : "MicrosoftGraph",
		},
	],
	fallbackReviewers : [
		{
			query : "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
			queryType : "MicrosoftGraph",
		},
		{
			query : "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
			queryType : "MicrosoftGraph",
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitionsById("accessReviewScheduleDefinition-id").instancesById("accessReviewInstance-id").stagesById("accessReviewStage-id").patch(requestBody);
}


```