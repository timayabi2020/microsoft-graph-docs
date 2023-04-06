---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'",
	}
};

const result = async () => {
	await graphServiceClient.appCatalogs.teamsApps.get(configuration);
}


```