---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AuthorizationPolicy = {
	allowedToUseSSPR : true,
};

const result = async () => {
	await graphServiceClient.policies.authorizationPolicy.patch(requestBody);
}


```