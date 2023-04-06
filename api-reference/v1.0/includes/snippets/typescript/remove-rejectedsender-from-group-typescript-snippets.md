---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		id: "https://graph.microsoft.com/v1.0/users/{user-id}",
	}
};

async () => {
	await graphServiceClient.groupsById("group-id").rejectedSenders.$ref.delete(configuration);
}


```