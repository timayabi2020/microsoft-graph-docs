---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationToRecipientsPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.EntityUrl,
		value : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/{teamsAppId}",
	},
	activityType : "pendingFinanceApprovalRequests",
	previewText : {
		content : "Internal spending team has a pending finance approval requests",
	},
	recipients : [
		{
			"@odata.type" : "microsoft.graph.aadUserNotificationRecipient",
			additionalData : {
				"userId" : "569363e2-4e49-4661-87f2-16f245c5d66a",
			},
		},
		{
			"@odata.type" : "microsoft.graph.aadUserNotificationRecipient",
			additionalData : {
				"userId" : "ab88234e-0874-477c-9638-d144296ed04f",
			},
		},
		{
			"@odata.type" : "microsoft.graph.aadUserNotificationRecipient",
			additionalData : {
				"userId" : "01c64f53-69aa-42c7-9b7f-9f75195d6bfc",
			},
		},
	],
	templateParameters : [
		{
			name : "pendingRequestCount",
			value : "5",
		},
	],
};

const result = async () => {
	await graphServiceClient.teamwork.sendActivityNotificationToRecipients.post(requestBody);
}


```