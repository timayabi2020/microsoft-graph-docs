---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "distributionMethod eq 'organization'",
	}
};

const result = async () => {
	await graphServiceClient.appCatalogs.teamsApps.get(configuration);
}


```