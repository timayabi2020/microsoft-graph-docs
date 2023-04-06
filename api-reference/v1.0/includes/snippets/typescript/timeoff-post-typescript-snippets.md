---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TimeOff = {
	userId : "c5d0c76b-80c4-481c-be50-923cd8d680a1",
	sharedTimeOff : {
		timeOffReasonId : "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
		startDateTime : new Date("2019-03-11T07:00:00Z"),
		endDateTime : new Date("2019-03-12T07:00:00Z"),
		theme : ScheduleEntityTheme.White,
	},
	draftTimeOff : {
		timeOffReasonId : "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
		startDateTime : new Date("2019-03-11T07:00:00Z"),
		endDateTime : new Date("2019-03-12T07:00:00Z"),
		theme : ScheduleEntityTheme.Pink,
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timesOff.post(requestBody);
}


```