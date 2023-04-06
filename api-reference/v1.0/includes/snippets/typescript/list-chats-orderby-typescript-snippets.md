---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		orderby: ["lastMessagePreview/createdDateTime desc"],
	}
};

const result = async () => {
	await graphServiceClient.chats.get(configuration);
}


```