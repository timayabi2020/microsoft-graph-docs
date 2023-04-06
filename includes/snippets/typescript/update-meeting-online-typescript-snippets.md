---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Event = {
	isOnlineMeeting : true,
	onlineMeetingProvider : OnlineMeetingProviderType.TeamsForBusiness,
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").patch(requestBody);
}


```