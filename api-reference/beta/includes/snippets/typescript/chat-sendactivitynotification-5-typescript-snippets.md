---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.EntityUrl,
		value : "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2",
	},
	activityType : "taskCreated",
	previewText : {
		content : "New Task Created",
	},
	recipient : {
		"@odata.type" : "microsoft.graph.chatMembersNotificationRecipient",
		additionalData : {
			"chatId" : "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2",
		},
	},
	templateParameters : [
		{
			name : "taskId",
			value : "Task 12322",
		},
	],
};

const result = async () => {
	await graphServiceClient.chatsById("chat-id").sendActivityNotification.post(requestBody);
}


```