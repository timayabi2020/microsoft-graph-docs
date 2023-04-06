---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.EntityUrl,
		value : "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}",
	},
	activityType : "reservationUpdated",
	previewText : {
		content : "You have moved up the queue",
	},
	recipient : {
		"@odata.type" : "microsoft.graph.aadUserNotificationRecipient",
		additionalData : {
			"userId" : "jacob@contoso.com",
		},
	},
	templateParameters : [
		{
			name : "reservationId",
			value : "TREEE433",
		},
		{
			name : "currentSlot",
			value : "23",
		},
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").sendActivityNotification.post(requestBody);
}


```