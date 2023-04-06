---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DismissPostRequestBody = {
	userIds : [
		"4628e7df-dff3-407c-a08f-75f08c0806dc",
	],
};

const result = async () => {
	await graphServiceClient.identityProtection.riskyUsers.dismiss.post(requestBody);
}


```