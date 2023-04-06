---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.EntityUrl,
		value : "https://graph.microsoft.com/v1.0/chats/{chatId}",
	},
	activityType : "taskCreated",
	previewText : {
		content : "New Task Created",
	},
	recipient : {
		"@odata.type" : "microsoft.graph.aadUserNotificationRecipient",
		additionalData : {
			"userId" : "569363e2-4e49-4661-87f2-16f245c5d66a",
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