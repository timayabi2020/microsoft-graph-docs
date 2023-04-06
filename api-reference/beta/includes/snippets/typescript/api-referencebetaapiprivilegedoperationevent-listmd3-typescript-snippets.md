---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "(creationDateTime ge 2017-06-25T07:00:00Z) and ",
		count: true,
		orderby: ["creationDateTime desc"],
	}
};

const result = async () => {
	await graphServiceClient.privilegedOperationEvents.get(configuration);
}


```