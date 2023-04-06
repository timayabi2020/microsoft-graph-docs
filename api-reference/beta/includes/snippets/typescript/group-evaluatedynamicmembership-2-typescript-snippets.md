---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EvaluateDynamicMembershipPostRequestBody = {
	memberId : "319b41e8-d9e4-42f8-bdc9-741113f48b33",
	membershipRule : "(user.displayName -startsWith \"EndTestUser\")",
};

const result = async () => {
	await graphServiceClient.groups.evaluateDynamicMembership.post(requestBody);
}


```