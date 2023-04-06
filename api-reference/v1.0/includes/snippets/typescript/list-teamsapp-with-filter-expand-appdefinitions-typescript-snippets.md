---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "id eq '876df28f-2e78-423b-94a5-44181bd0e225'",
		expand: ["appDefinitions"],
	}
};

const result = async () => {
	await graphServiceClient.appCatalogs.teamsApps.get(configuration);
}


```