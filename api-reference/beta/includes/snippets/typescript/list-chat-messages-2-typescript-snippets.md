---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		top: 2,
		orderby: ["lastModifiedDateTime desc"],
		filter: "lastModifiedDateTime ge 2022-09-22T00:00:00.000Z and lastModifiedDateTime le 2022-09-24T00:00:00.000Z",
	}
};

const result = async () => {
	await graphServiceClient.chatsById("chat-id").messages.get(configuration);
}


```