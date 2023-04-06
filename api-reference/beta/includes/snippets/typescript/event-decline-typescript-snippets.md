---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DeclinePostRequestBody = {
	comment : "I won't be able to make this week. How about next week?",
	sendResponse : true,
	proposedNewTime : {
		start : {
			dateTime : "2019-12-02T18:00:00",
			timeZone : "Pacific Standard Time",
		},
		end : {
			dateTime : "2019-12-02T19:00:00",
			timeZone : "Pacific Standard Time",
		},
	},
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").decline.post(requestBody);
}


```