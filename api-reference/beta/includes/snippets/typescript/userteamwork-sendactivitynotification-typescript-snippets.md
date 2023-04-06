---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SendActivityNotificationPostRequestBody = {
	topic : {
		source : TeamworkActivityTopicSource.EntityUrl,
		value : "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}",
	},
	activityType : "taskCreated",
	previewText : {
		content : "New Task Created",
	},
	templateParameters : [
		{
			name : "taskId",
			value : "Task 12322",
		},
	],
};

const result = async () => {
	await graphServiceClient.usersById("user-id").teamwork.sendActivityNotification.post(requestBody);
}


```