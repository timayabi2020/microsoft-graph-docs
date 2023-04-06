---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Event = {
	originalStartTimeZone : "originalStartTimeZone-value",
	originalEndTimeZone : "originalEndTimeZone-value",
	responseStatus : {
		response : ResponseType.None,
		time : new Date("datetime-value"),
	},
	uid : "iCalUId-value",
	reminderMinutesBeforeStart : 99,
	isReminderOn : true,
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").eventsById("event-id").patch(requestBody);
}


```