---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["isOnlineMeeting","onlineMeetingProvider","onlineMeeting"],
	}
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").get(configuration);
}


```