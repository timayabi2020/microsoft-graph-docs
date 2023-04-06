---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.EntityUrl,
		value : "https://graph.microsoft.com/v1.0/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7",
	},
	activityType : "pendingFinanceApprovalRequests",
	previewText : {
		content : "Internal spending team has a pending finance approval requests",
	},
	recipient : {
		"@odata.type" : "microsoft.graph.channelMembersNotificationRecipient",
		additionalData : {
			"teamId" : "e8bece96-d393-4b9b-b8da-69cedef1a7e7",
			"channelId" : "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2",
		},
	},
	templateParameters : [
		{
			name : "pendingRequestCount",
			value : "5",
		},
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").sendActivityNotification.post(requestBody);
}


```