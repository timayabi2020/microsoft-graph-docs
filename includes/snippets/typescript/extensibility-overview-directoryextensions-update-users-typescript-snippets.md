---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : User = {
	additionalData : {
		extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable : null,
		"extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker" : "E4",
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").patch(requestBody);
}


```