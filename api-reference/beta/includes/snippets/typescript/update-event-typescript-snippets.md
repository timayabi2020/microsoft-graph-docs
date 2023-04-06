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
		time : new Date("2016-10-19T10:37:00Z"),
	},
	recurrence : null,
	uid : "iCalUId-value",
	reminderMinutesBeforeStart : 99,
	isOnlineMeeting : true,
	onlineMeetingProvider : OnlineMeetingProviderType.TeamsForBusiness,
	isReminderOn : true,
	hideAttendees : false,
	categories : [
		"Red category",
	],
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").patch(requestBody);
}


```