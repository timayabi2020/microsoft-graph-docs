---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "appId eq '00000002-0000-0000-c000-000000000000'",
	}
};

const result = async () => {
	await graphServiceClient.servicePrincipals.get(configuration);
}


```