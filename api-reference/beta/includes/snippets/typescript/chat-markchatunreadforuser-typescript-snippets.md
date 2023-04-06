---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MarkChatUnreadForUserPostRequestBody = {
	user : {
		id : "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2",
		additionalData : {
			"tenantId" : "2a690434-97d9-4eed-83a6-f5f13600199a",
		},
	},
	lastMessageReadDateTime : new Date("2021-05-27T22:13:01.577Z"),
};

const result = async () => {
	await graphServiceClient.chatsById("chat-id").markChatUnreadForUser.post(requestBody);
}


```