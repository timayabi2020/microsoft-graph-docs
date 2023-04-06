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
		"@odata.type" : "microsoft.graph.channelMembersNotificationRecipient",
		additionalData : {
			"teamId" : "7155e3c8-175e-4311-97ef-572edc3aa3db",
			"channelId" : "19:0ea5de04de4743bcb4cd20cb99235d99@thread.tacv2",
		},
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").sendActivityNotification.post(requestBody);
}


```