---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Subscription = {
	expirationDateTime : new Date("2016-03-22T11:00:00.0000000Z"),
};

const result = async () => {
	await graphServiceClient.subscriptionsById("subscription-id").patch(requestBody);
}


```