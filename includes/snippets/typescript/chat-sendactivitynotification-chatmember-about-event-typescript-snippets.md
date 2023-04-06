---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.Text,
		value : "Weekly Virtual Social",
		webUrl : "Teams webUrl",
	},
	previewText : {
		content : "It will be fun!",
	},
	activityType : "eventCreated",
	recipient : {
		"@odata.type" : "microsoft.graph.chatMembersNotificationRecipient",
		additionalData : {
			"chatId" : "19:d65713bc498c4a428c71ef9353e6ce20@thread.v2",
		},
	},
};

const result = async () => {
	await graphServiceClient.chatsById("chat-id").sendActivityNotification.post(requestBody);
}


```