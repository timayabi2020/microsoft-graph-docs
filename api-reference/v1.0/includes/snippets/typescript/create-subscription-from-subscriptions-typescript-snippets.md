---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Subscription = {
	changeType : "created",
	notificationUrl : "https://webhook.azurewebsites.net/api/send/myNotifyClient",
	resource : "me/mailFolders('Inbox')/messages",
	expirationDateTime : new Date("2016-11-20T18:23:45.9356913Z"),
	clientState : "secretClientValue",
	latestSupportedTlsVersion : "v1_2",
};

const result = async () => {
	await graphServiceClient.subscriptions.post(requestBody);
}


```