---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "mailEnabled eq true",
		search: "\"displayName:OneVideo\"",
	}
};

const result = async () => {
	await graphServiceClient.groups.get(configuration);
}


```