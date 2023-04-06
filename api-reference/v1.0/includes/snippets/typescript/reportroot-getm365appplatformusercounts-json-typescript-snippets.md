---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		format: "application/json",
	}
};

const result = async () => {
	await graphServiceClient.reports.getM365AppPlatformUserCounts(period='{period}').get(configuration);
}


```