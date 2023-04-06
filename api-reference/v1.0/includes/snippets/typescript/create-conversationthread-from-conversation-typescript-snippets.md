---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConversationThread = {
	topic : "Take your wellness days and rest",
	posts : [
		{
			body : {
				contentType : BodyType.Html,
				content : "Waiting for the summer holidays.",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").conversationsById("conversation-id").threads.post(requestBody);
}


```