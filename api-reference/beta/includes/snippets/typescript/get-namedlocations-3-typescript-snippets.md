---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "createdDateTime ge 2019-09-01T00:00:00Z",
	}
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.namedLocations.get(configuration);
}


```