---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Subscription = {
	changeType : "created",
	notificationUrl : "https://webhook.azurewebsites.net/api/send/myNotifyClient",
	resource : "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages",
	expirationDateTime : new Date("2021-07-07T21:42:18.2257768+00:00"),
	clientState : "secretClientState",
};

const result = async () => {
	await graphServiceClient.subscriptions.post(requestBody);
}


```