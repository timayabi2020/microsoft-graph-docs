---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewInstanceDecisionItem = {
	decision : "Approve",
	justification : "This person is still on my team",
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitionsById("accessReviewScheduleDefinition-id").instancesById("accessReviewInstance-id").stagesById("accessReviewStage-id").decisionsById("accessReviewInstanceDecisionItem-id").patch(requestBody);
}


```