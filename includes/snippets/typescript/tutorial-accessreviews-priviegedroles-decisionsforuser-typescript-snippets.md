---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Decision = {
	additionalData : {
		"decision" : "Deny",
		"justification" : "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'",
	},
};

async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitionsById("accessReviewScheduleDefinition-id").instancesById("accessReviewInstance-id").decisionsById("accessReviewInstanceDecisionItem-id").post(requestBody);
}


```