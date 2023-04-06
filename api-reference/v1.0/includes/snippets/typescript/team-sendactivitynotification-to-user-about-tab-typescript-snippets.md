---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.EntityUrl,
		value : "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}",
	},
	activityType : "reservationUpdated",
	previewText : {
		content : "You have moved up the queue",
	},
	recipient : {
		"@odata.type" : "microsoft.graph.aadUserNotificationRecipient",
		additionalData : {
			"userId" : "569363e2-4e49-4661-87f2-16f245c5d66a",
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