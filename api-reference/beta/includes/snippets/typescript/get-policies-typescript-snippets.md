---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'",
	}
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.policies.get(configuration);
}


```