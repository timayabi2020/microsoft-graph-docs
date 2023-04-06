---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		expand: ["microsoft.graph.eventMessage/event"],
	}
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").get(configuration);
}


```