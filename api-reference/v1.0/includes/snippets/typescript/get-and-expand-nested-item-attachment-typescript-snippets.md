---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		expand: ["microsoft.graph.itemattachment/item"],
	}
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachmentsById("attachment-id").get(configuration);
}


```