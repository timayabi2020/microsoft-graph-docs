---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SnoozeReminderPostRequestBody = {
	newReminderTime : {
		dateTime : "2016-10-19T10:37:00Z",
		timeZone : "timeZone-value",
	},
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").snoozeReminder.post(requestBody);
}


```