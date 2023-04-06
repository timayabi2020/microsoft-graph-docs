---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PermissionGrantPolicy = {
	id : "my-custom-consent-policy",
	displayName : "Custom application consent policy",
	description : "A custom permission grant policy to customize conditions for granting consent.",
};

const result = async () => {
	await graphServiceClient.policies.permissionGrantPolicies.post(requestBody);
}


```