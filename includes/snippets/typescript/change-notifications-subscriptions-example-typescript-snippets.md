---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Subscription = {
	changeType : "created,updated",
	notificationUrl : "https://webhook.azurewebsites.net/notificationClient",
	resource : "/me/mailfolders('inbox')/messages",
	expirationDateTime : new Date("2016-03-20T11:00:00.0000000Z"),
	clientState : "SecretClientState",
};

const result = async () => {
	await graphServiceClient.subscriptions.post(requestBody);
}


```