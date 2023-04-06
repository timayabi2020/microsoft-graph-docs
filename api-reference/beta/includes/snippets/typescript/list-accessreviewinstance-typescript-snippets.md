---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		top: 100,
		skip: 0,
	}
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitionsById("accessReviewScheduleDefinition-id").instances.get(configuration);
}


```