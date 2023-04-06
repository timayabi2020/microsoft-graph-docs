---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.EntityUrl,
		value : "https://graph.microsoft.com/beta/teams/{teamId}",
	},
	activityType : "pendingFinanceApprovalRequests",
	previewText : {
		content : "Internal spending team has a pending finance approval requests",
	},
	recipient : {
		"@odata.type" : "microsoft.graph.aadUserNotificationRecipient",
		additionalData : {
			"userId" : "569363e2-4e49-4661-87f2-16f245c5d66a",
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