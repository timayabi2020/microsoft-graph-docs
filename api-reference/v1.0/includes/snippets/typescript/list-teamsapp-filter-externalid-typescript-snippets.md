---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'",
	}
};

const result = async () => {
	await graphServiceClient.appCatalogs.teamsApps.get(configuration);
}


```